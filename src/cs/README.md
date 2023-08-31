# C#

## Notes

- The `src/cs` directory is for housing all C# code including production and test code.
- The C# `.sln` sits in this directory.
- Each C# project `.csproj` is a folder which said folder sits in this directory.
- The `Directory.Build.props` and `Directory.Build.targets` files apply common things to each `.csproj` that is in a folder which said folder sits in this directory.
- To turn on or off specific analyzers, please use the `Analyzers.globalconfig` in this directory; it will be applied to all `.csproj` in folders or sub-folders of this directory.
- If you want sub-folders to organize the C# code, include a `Directory.Build.props` file and `Directory.Build.targets` file that reference the files with the same name that sit in this directory. You may also wish to have a `Analyzers.globalconfig` for only specific sub-folders.