# setup-wasi-sdk

A GitHub Action that installs the [wasi-sdk](https://github.com/WebAssembly/wasi-sdk) toolchain on /opt/wasi-sdk on the Runner.

This action itself is licensed under the Unlicense. Keep in mind wasi-sdk and it's components, including LLVM, Clang, and [wasi-libc](https://github.com/WebAssembly/wasi-libc), have their own licenses.

## Usage

```yaml
- uses: redbluegreenhat/setup-wasi-sdk@main
  with:
    # Version of the SDK to install.
    # Optional, but it is highly recommended you set this in your workflow explicitly
    # By default, download and installs wasi-sdk-27
    sdk-version: 27
```

If you want an example of it being used, check out the workflow for my [wasi-blog](https://github.com/redbluegreenhat/wasi-blog/blob/main/.github/workflows/main.yml) repository.
