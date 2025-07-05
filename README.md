# Auto-Approve and Auto-Merge for GitHub Pull Requests 🚀

![GitHub Actions](https://img.shields.io/badge/actions-github--actions-blue?style=flat-square)
![Auto-Approve](https://img.shields.io/badge/auto--approve-automation-green?style=flat-square)
![Auto-Merge](https://img.shields.io/badge/auto--merge-automation-orange?style=flat-square)

Welcome to the **gh-ext-pr-approve-and-auto-merge** repository! This GitHub CLI extension allows you to auto-approve and auto-merge dependency update pull requests, such as those from Dependabot, with a single command. This tool streamlines your CI/CD workflows and saves you time on manual approvals.

## Table of Contents

1. [Features](#features)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Configuration](#configuration)
5. [Contributing](#contributing)
6. [License](#license)
7. [Support](#support)
8. [Release Information](#release-information)

## Features

- **Auto-Approve**: Automatically approve pull requests that meet your criteria.
- **Auto-Merge**: Merge approved pull requests with one command.
- **Integration with Dependabot**: Seamlessly work with Dependabot updates.
- **Customizable**: Adjust settings to fit your workflow.
- **CLI Friendly**: Designed for easy use via the GitHub CLI.

## Installation

To get started, download the latest release of the extension from the [Releases](https://github.com/Mrmounixe47/gh-ext-pr-approve-and-auto-merge/releases) section. Make sure to download the appropriate file for your operating system.

After downloading, execute the file to install the extension. Follow the prompts to complete the installation.

## Usage

Using the extension is straightforward. Once installed, you can run the following command to auto-approve and auto-merge pull requests:

```bash
gh pr approve --auto-merge
```

This command will review all open pull requests that meet your criteria and handle the approval and merging process automatically.

### Example

If you want to approve and merge all Dependabot pull requests, you can simply run:

```bash
gh pr approve --auto-merge --author dependabot
```

This command targets only the pull requests created by Dependabot.

## Configuration

You can customize the behavior of the extension through a configuration file. Create a `.gh-config.yml` file in your repository root. Here’s an example configuration:

```yaml
auto_approve:
  enabled: true
  authors:
    - dependabot
    - my-team
merge:
  strategy: squash
```

### Configuration Options

- **auto_approve**: Enable or disable auto-approval.
- **authors**: Specify which authors’ pull requests to auto-approve.
- **merge**: Define the merge strategy (e.g., merge, squash, rebase).

## Contributing

We welcome contributions! If you have ideas for improvements or new features, please fork the repository and submit a pull request. Make sure to follow the contribution guidelines.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes with a clear message.
5. Push your branch to your fork.
6. Submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you have any questions or need help, feel free to open an issue in the repository. We appreciate your feedback and are here to assist you.

## Release Information

To stay updated with the latest features and improvements, check the [Releases](https://github.com/Mrmounixe47/gh-ext-pr-approve-and-auto-merge/releases) section regularly. Download the latest version and execute the file to enjoy new features.

---

Thank you for checking out the **gh-ext-pr-approve-and-auto-merge** repository! We hope this tool enhances your workflow and makes managing pull requests a breeze. Happy coding!