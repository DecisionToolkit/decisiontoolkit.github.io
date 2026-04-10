# Command-line

> Cheat sheet

|   Action | Decision<br/>model | Decision<br/>table | FEEL<br/>expression | Built-in<br/>examples |
|---------:|:------------------:|:------------------:|:-------------------:|:---------------------:|
| Evaluate |       [edm]        |       [edt]        |        [efe]        |                       | 
|    Parse |       [pdm]        |       [pdt]        |        [pfe]        |                       |
|     Test |       [tdm]        |       [tdt]        |        [tfe]        |                       |
|   Export |       [xdm]        |       [xdt]        |        [xfe]        |                       |
|    Serve |       [srv]        |                    |                     |                       |
|     Save |                    |                    |                     |         [exs]         |

## Commands

### srv

> Runs ^dt as a service and serves DMN decision models

To display all available options of the [srv] command, run:

```shell
dsntk help srv
```

For more details, refer to [Serving DMN models][srv].

### edm

> Evaluates DMN decision model

To display all available options of the [edm] command, run:

```shell
dsntk help edm
```

For more details, refer to [Evaluating DMN models][edm].

### edt

> Evaluates decision table

To display all available options of the [edt] command, run:

```shell
dsntk help edt
```

For more details, refer to [Evaluating decision tables][edt].

### efe

> Evaluates FEEL expression

To display all available options of the [efe] command, run:

```shell
dsntk help efe
```

For more details, refer to [Evaluating FEEL expressions][efe].

### pdm

> Parses DMN model

To display all available options of the [pdm] command, run:

```shell
dsntk help pdm
```

For more details, refer to [Parsing DMN models][pdm].

### pdt

> Parses decision table

To display all available options of the [pdt] command, run:

```shell
dsntk help pdt
```

For more details, refer to [Parsing decision tables][pdt].

### pfe

> Parses FEEL expression

To display all available options of the [pfe] command, run:

```shell
dsntk help pfe
```

For more details, refer to [Parsing FEEL expressions][pfe].

### tdm

> Tests DMN model

To display all available options of the [tdm] command, run:

```shell
dsntk help tdm
```

For more details, refer to [Testing DMN models][tdm].

### tdt

> Tests decision table

To display all available options of the [tdt] command, run:

```shell
dsntk help tdt
```

For more details, refer to [Testing decision tables][tdt].

### tfe

> Tests FEEL expression

To display all available options of the [tfe] command, run:

```shell
dsntk help tfe
```

For more details, refer to [Testing FEEL expressions][tfe].

### xdm

> Exports DMN model

To display all available options of the [xdm] command, run:

```shell
dsntk help xdm
```

For more details, refer to [Exporting DMN models][xdm].

### xdt

> Exports decision table

To display all available options of the [xdt] command, run:

```shell
dsntk help xdt
```

For more details, refer to [Exporting decision tables][xdt].

### xfe

> Exports FEEL expression

To display all available options of the [xfe] command, run:

```shell
dsntk help xfe
```

For more details, refer to [Exporting FEEL expressions][xfe].

### exs

> Saves the examples

To display all available options of the [exs] command, run:

```shell
dsntk help exs
```

For more details, refer to [Saving examples][exs].

## Options

Below is a list of all ^dt options.

### help

Print help:

```shell
dsntk --help
```

or short:

```shell
dsntk -h
```

### version

Print version:

```shell
dsntk --version
```

or short:

```shell
dsntk -V
```

[edm]: commands/edm.md
[edt]: commands/edt.md
[efe]: commands/efe.md
[pdm]: commands/pdm.md
[pdt]: commands/pdt.md
[pfe]: commands/pfe.md
[tdm]: commands/tdm.md
[tdt]: commands/tdt.md
[tfe]: commands/tfe.md
[xdm]: commands/xdm.md
[xdt]: commands/xdt.md
[xfe]: commands/xfe.md
[srv]: commands/srv.md
[exs]: commands/exs.md 
