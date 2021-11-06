[![Go Reference](https://pkg.go.dev/badge/github.com/tj-actions/auto-doc.svg)](https://pkg.go.dev/github.com/tj-actions/auto-doc)
[![CI](https://github.com/tj-actions/auto-doc/workflows/CI/badge.svg)](https://github.com/tj-actions/auto-doc/actions?query=workflow%3ACI)
[![Update release version.](https://github.com/tj-actions/auto-doc/workflows/Update%20release%20version./badge.svg)](https://github.com/tj-actions/auto-doc/actions?query=workflow%3A%22Update+release+version.%22)
[![Public workflows that use this action.](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi-tj-actions1.vercel.app%2Fapi%2Fgithub-actions%2Fused-by%3Faction%3Dtj-actions%2Fauto-doc%26badge%3Dtrue)](https://github.com/search?o=desc\&q=tj-actions+auto-doc+language%3AYAML\&s=\&type=Code)


[![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu\&logoColor=white)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)
[![Mac OS](https://img.shields.io/badge/mac%20os-000000?logo=macos\&logoColor=F0F0F0)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)
[![Windows](https://img.shields.io/badge/Windows-0078D6?logo=windows\&logoColor=white)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)

## auto-doc

Auto generate documentation from actions.yml like [this](#inputs) by simply adding `Inputs` and/or `Outputs` [`H2` header](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#headers) to your `README.md`.

## Usage

```yaml
...
    steps:
      - uses: actions/checkout@v2
      - name: Run auto-doc
        uses: tj-actions/auto-doc@v1.0.1
```

## Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section --> 

| INPUT  | REQUIRED |  DEFAULT   |         DESCRIPTION         |
|--------|----------|------------|-----------------------------|
| action | true     | action.yml | Path to the action.yml file |
| output | true     | README.md  | Output file                 |

<!-- AUTO-DOC-INPUT:END -->









### 👆 This is autogenerated 👆 using:

`action.yml`

```yaml
...
inputs:
  action:
    description: 'Path to the action.yml file'
    required: true
    default: action.yml
  output:
    description: 'Output file'
    required: true
    default: README.md

runs:
  ...
branding:
  ...
```

### Using CLI

#### Installation

Run

    go get -u github.com/tj-actions/auto-doc

command line options

    auto-doc -h                                                                                                                               [5/11/21 | 5:26:52]
    Auto generate documentation for your github action.

    Usage:
      auto-doc [flags]

    Flags:
          --action string   action config file (default "action.yml")
      -h, --help            help for auto-doc
          --output string   Output file (default "README.md")

*   Free software: [Apache License 2.0](LICENSE)

If you feel generous and want to show some extra appreciation:

[![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]

[buymeacoffee]: https://www.buymeacoffee.com/jackton1

[buymeacoffee-shield]: https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png

## Credits

This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) using [cookiecutter-action](https://github.com/tj-actions/cookiecutter-action)

*   [cobra](https://github.com/spf13/cobra/cobra)
*   [gobadge](https://github.com/AlexBeauchemin/gobadge)
*   [gobinaries](https://github.com/tj/gobinaries)

## Report Bugs

Report bugs at https://github.com/tj-actions/auto-doc/issues.

If you are reporting a bug, please include:

*   Your operating system name and version.
*   Any details about your workflow that might be helpful in troubleshooting.
*   Detailed steps to reproduce the bug.
