[![](https://img.shields.io/nuget/v/soenneker.libraries.git.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.git.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.git.windows/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.git.windows/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.git.windows.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.git.windows/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.git.windows/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.git.windows/actions/workflows/codeql.yml)

# Soenneker.Libraries.Git.Windows

A self-contained Git distribution packaged for Windows x64 .NET applications.

## Install

```bash
dotnet add package Soenneker.Libraries.Git.Windows
```

The distribution is copied beneath the application output directory. Use the command entry point so Git can locate the bundled helper programs:

```csharp
string git = Path.Combine(
    AppContext.BaseDirectory,
    "Resources", "win-x64", "git", "cmd", "git.exe");
```

Pass each Git argument through `ProcessStartInfo.ArgumentList`, especially repository paths, refs, and commit messages derived from input. Set the working directory explicitly when a command should operate on a particular repository.

This package contains Windows x64 assets and does not provide a managed Git API or select binaries for other platforms.
