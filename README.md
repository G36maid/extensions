# Zed Extensions

This is the central repository containing the extensions available for [Zed](https://zed.dev/).

## Getting started

See the [Developing Extensions](https://zed.dev/docs/extensions/developing-extensions) docs for how to develop and publish your extension

Looking for extension ideas? Check out:

- [Top theme requests](https://github.com/zed-industries/extensions/issues?q=is%3Aissue+is%3Aopen+label%3Atheme+sort%3Areactions-%2B1-desc)
- [Top language requests](https://github.com/zed-industries/extensions/issues?q=is%3Aissue+is%3Aopen+label%3Alanguage+sort%3Areactions-%2B1-desc)

If an issue requesting an extension is tagged with the `needs infrastructure` label, it indicates that the extension cannot currently be developed due to the absence of necessary system infrastructure.

## CI Workflow

This repository includes a basic GitHub Actions CI workflow at `.github/workflows/ci.yml` that:

- Runs on every push and pull request to any branch
- Automatically detects and builds Node.js/TypeScript projects (active for this repository)
- Includes commented templates for easy customization for other language stacks

### Customizing the CI for Different Languages

The CI workflow includes ready-to-use templates for common language stacks. To customize:

1. **Node.js/TypeScript** (currently active): No changes needed
2. **Python**: Uncomment the Python section and customize as needed
3. **Rust**: Uncomment the Rust section and customize as needed
4. **Go**: Uncomment the Go section and customize as needed
5. **Java/Maven**: Uncomment the Java section and customize as needed
6. **C/C++**: Uncomment the C/C++ section and customize as needed

Each template includes:

- Language-specific setup and caching
- Dependency installation
- Linting/formatting checks
- Building
- Testing

### Testing the Workflow

The workflow will automatically run when you:

- Push commits to any branch
- Open a pull request
- Update an existing pull request

You can also test it locally by running the individual commands from the workflow on your machine.
