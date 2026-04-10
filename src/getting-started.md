# Getting started

^dt provides a set of examples ready to play with.

To install examples in `examples` directory, run:

```shell
dsntk exs examples
```

For more details, refer to [Saving examples][exs].

## Evaluate example FEEL expression

```shell
cd examples/e1
```

```shell
dsntk efe e1.ctx e1.feel
```

Output:

```text
3
```

For more details, refer to [Evaluating FEEL expressions][efe].

## Evaluate example DMN model

```shell
cd examples/e2
```

```shell
dsntk edm e2.ctx e2.dmn -i "Greeting Message"
```

Output:

```text
"Hello John Doe"
```

For more details, refer to [Evaluating DMN models][edm].

## Evaluate example decision table

```shell
cd examples/e3
```

```shell
dsntk edt e3.ctx e3.dtb
```

Output:

```text
0.15
```

For more details, refer to [Evaluating decision tables][edt].

## Serve example DMN model

```shell
cd examples/e2
```

```shell
dsntk srv -v -H 127.0.0.1 -D .
```

Output:

```text
Found 1 model.
Loaded 1 model.
Deployed 1 invocable.

Deployed invocables:
  io/dsntk/2_0001/compliance-level-2-test-0001/Greeting%20Message

dsntk 127.0.0.1:22022
```

Open a new terminal window and run:

```shell
curl -s -d "{\"Full Name\":\"John Doe\"}" \
     -H "Content-Type: application/json" \
     -X POST http://127.0.0.1:22022/evaluate/io/dsntk/2_0001/compliance-level-2-test-0001/Greeting%20Message
```

Output:

```text
{"data":"Hello John Doe"}
```

For more details, refer to [Serving DMN models][srv].

[srv]: ./commands/command-srv.md
[edt]: ./commands/command-edt.md
[edm]: ./commands/command-edm.md
[efe]: ./commands/command-efe.md
[exs]: ./commands/command-exs.md

^checked
