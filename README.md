[![](https://img.shields.io/nuget/v/soenneker.libraries.git.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.git.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.git.windows/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.git.windows/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.git.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.git.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.git.windows/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.git.windows/actions/workflows/codeql.yml)

# Soenneker.Libraries.Git.Windows

Provides a statically linked git executable for Windows.

## Install

```bash
dotnet add package Soenneker.Libraries.Git.Windows
```

## What it provides

- Provides a statically linked git executable for Windows.
- The file is copied to the output directory, and located at the relative path: `Resources\`.

## How to use it

After installation, resolve the packaged file from the output-relative path above. The package deploys the asset but does not invoke it for you.
