<div style="font-size:3em;color:#33691E;font-weight:600;margin-top:10pt;">ÐecisionToolkit</div>
<span style="font-size:1.5em;color:gray;">Design, test and execute decisions</span>

<div style="display:flex;justify-content:center;background-color:#33691E;margin-top:16px">
<div style="max-width:200px;">

![logo](./images/decision-toolkit.svg)

</div>
</div>

^dt is a set of tools designed to build, test and evaluate decision models, constructed basing
on the ^DecisionModelandNotation specification,
which is an industry standard governed by the ^OMG.

^dt aims to be performant, reliable, and fully compliant with the ^DMN specification,
ensuring accurate evaluation of decision models. All tools are implemented in ^rust,
a programming language known for its security, efficiency and reliability.

^dt offers a range of features, including DMN models evaluation, decision tables evaluation,
and FEEL expressions evaluation. It also includes functionality for parsing, validating,
and recognizing DMN models, decision tables, and FEEL expressions.
Users can test DMN models, decision tables, and FEEL expressions, and export them to HTML.

## Features

- [Serving DMN models](commands/srv.md)
- [Evaluating DMN models](commands/edm.md)
- [Evaluating decision tables](commands/edt.md)
- [Evaluating FEEL expressions](commands/efe.md)
- [Parsing DMN models](commands/pdm.md)
- [Parsing decision tables](commands/pdt.md)
- [Parsing FEEL expressions](commands/pfe.md)
- [Testing DMN models](commands/tdm.md)
- [Testing decision tables](commands/tdt.md)
- [Testing FEEL expressions](commands/tfe.md)
- [Exporting DMN models](commands/xdm.md)
- [Exporting decision tables](commands/xdt.md)
- [Exporting FEEL expressions](commands/xfe.md)

## Status

^dt is **PRODUCTION READY**, although some features may still be refined or changed based on testing and user feedback.
We encourage users to try ^dt and share their feedback to help us enhance its usability and performance.

^note
> This book assumes you’re using ^dt version **^dsntk-ver** or later.
> Please visit [Installation](./installation.md) chapter to learn how to install or update ^dt.

^contrib

^checked
