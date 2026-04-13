<div style="font-size:3em;color:#33691E;font-weight:600;margin-top:10pt;">ÐecisionToolkit</div>
<span style="font-size:1.5em;color:gray;">Design and execute decisions</span>

<div style="display:flex;justify-content:center;background-color:#33691E;margin-top:16px">
<div style="max-width:200px;">

![logo](./images/decision-toolkit.svg)

</div>
</div>

^dt is a set of tools for designing, testing and executing decision models
based on the ^DMN specification, an industry standard governed by ^OMG.

^dt aims to be performant, reliable, and fully compliant with the DMN specification,
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

## License

[mit-url]: https://opensource.org/licenses/MIT
[mit-license-url]: https://github.com/DecisionToolkit/dsntk/blob/main/LICENSE-MIT
[apache-url]: https://www.apache.org/licenses/LICENSE-2.0
[apache-license-url]: https://github.com/DecisionToolkit/dsntk/blob/main/LICENSE
[apache-notice-url]: https://github.com/DecisionToolkit/dsntk/blob/main/NOTICE

^dt is licensed under either of

- [MIT license][mit-url] (see [LICENSE-MIT][mit-license-url]) or
- [Apache License, Version 2.0][apache-url] (see [LICENSE][apache-license-url] and [NOTICE][apache-notice-url])

at your option.

## Contribution

Any contributions to ^dt are greatly appreciated.
All contributions intentionally submitted for inclusion in the work by you,
shall be dual licensed as above, without any additional terms or conditions.

## Versions

|  ^dt |   ^dsntk-ver |
|-----:|-------------:|
| ^DMN | **^dmn-ver** |

^footer
