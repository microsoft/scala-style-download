# Scalastyle Download Action [![Build](https://github.com/microsoft/scala-style-download/actions/workflows/ci.yml/badge.svg)](https://github.com/microsoft/scala-style-download/actions/workflows/ci.yml)


GitHub Action that downloads [Scalastyle](http://www.scalastyle.org/).

## When to use

This action is useful when you need to download Scalastyle to later examine your Scala code.

## How it works

1. The GitHub Action first downloads wget package to easily retrieve a file from an HTTP url.
2. The GitHub Action then retrieves Scalastyle jar package from and URL.

> Note: You can specify the URL from Scalastyle jar package. The default one in this Action is version 2.12

## Getting Started

### Prerequisites

* Make sure you have setup Java
* Make sure you have setup Scala

You can look for actions that help you with this pre-reqs in the Actions Marketplace.

### Usage

```yml
steps:
    - name: Download Scalastyle
      uses: microsoft/scalastyle-download@v1.0.0
      with:
        scalastyle-url: 'https://repo1.maven.org/maven2/org/scalastyle/scalastyle_2.12/1.0.0/scalastyle_2.12-1.0.0-batch.jar' # Default downloads version 2.12    
```

### Inputs

### Inputs

| Name | Description | Required | Default value |
| --- | --- | --- | --- |
| `scalastyle-url` | URL for Scalastyle jar package | false |https://repo1.maven.org/maven2/org/scalastyle/scalastyle_2.12/1.0.0/scalastyle_2.12-1.0.0-batch.jar |

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
