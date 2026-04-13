# Serving DMN models

The core functionality of the ^dt is serving DMN models.
The <Dmn/> specification precisely defines XML interchange format for decision models.
XML files containing decision models are loaded and processed by ^dt server and exposed
as a set of [JSON API] endpoints. Each endpoint represents a single invocable defined
in the decision model. Calling an endpoint is equivalent to executing a decision,
business knowledge model or decision service.

To explain in details, how to run and use the ^dt server, we assume
that the built-in examples are already saved in the `~/examples` directory
(see [Saving examples](exs.md) for details).

Change to the directory containing the examples:

```shell
cd ~/examples
```

## Running a server

To start ^dt server, type the following command:

```shell
dsntk srv
```

Expected output should look like this:

```text
Found 1 model.
Loaded 1 model.
Deployed 1 invocable.
dsntk 0.0.0.0:22022
```

^dt server is started. By default, ^dt server accepts connections from all available network
interfaces **0.0.0.0** and listens on port **22022**. During startup, the server scans the current directory
with all its subdirectories, and searches for decision models stored as XML files with `.dmn` extension.

In our example, during directory scanning, the ^dt server has found the `dm` directory
containing one decision model file named **dm.dmn**. This file was loaded, and one invocable
was deployed: decision named `Greeting Message`.

To stop the ^dt server, press **Ctrl+C**.

The list of all deployed invocables with endpoint names can be displayed during server startup
by specifying the option `-v` or `--verbose`, like shown below:

```shell
dsntk srv -v
```

```text
Found 1 model.
Loaded 1 model.
Deployed 1 invocable.

Deployed invocable:
  dm/org/decision-toolkit/greetings/Greeting%20Message

dsntk 0.0.0.0:22022
```

## Evaluating invocables

After starting the ^dt server, the deployed invocable can be evaluated by calling
its endpoint with required input data, using e.g. [curl](https://curl.se) tool.

In a new terminal window, run:

```shell
curl -s -w '\n' -d '{"Full Name":"Solomon L. Pollack"}' -H "Content-Type: application/json" -X POST http://0.0.0.0:22022/evaluate/dm/org/decision-toolkit/greetings/Greeting%20Message
```

Expected output:

```text
{"data":"Hello Solomon L. Pollack"}
```

The ^dt version of a [hello world](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program)
program could look like this:

```shell
curl -s -w '\n' -d '{"Full Name":"world"}' -H "Content-Type: application/json" -X POST http://0.0.0.0:22022/evaluate/dm/org/decision-toolkit/greetings/Greeting%20Message
```

Expected output:

```text
{"data":"Hello world"}
```

## Endpoint names

The [JSON API] endpoint for evaluating invocables exposed by the ^dt server is named `evaluate/`.

The full URL of the endpoint is composed of the following parts:

- the protocol:

  `http://` or `https://`

- host address:

  `0.0.0.0` or `127.0.0.1` or `my.domain.com/` alike

- endpoint name:

  `evaluate/`

- path built from directory names where the file containing the DMN model was found during startup scanning:

  `dm/`

- model namespace converted to RDNN-like path:

  `org/decision-toolkit/`

- model name:

  `greetings/`

- the name of the invocable:

  `Greeting%20Message`

All parts put together give the following URL of the endpoint:

```text
http://127.0.0.1:22022/evaluate/dm/org/decision-toolkit/greetings/Greeting%20Message
```

While not all characters are legal in URLs, there is `%20` between `Greeting` and `Message`,
which represents a space in [percent-encoding](https://en.wikipedia.org/wiki/Percent-encoding).
See [RFC3986](https://datatracker.ietf.org/doc/html/rfc3986#section-2.4) for more details.

[JSON API]: https://jsonapi.org

^footer
