# Regex Parser from Roslyn

This library exposes the internal regular expression parser used by Roslyn. It includes all the internal Roslyn types that are needed for this task. For the public types (such as `TextSpan`), the library references the NuGet package `Microsoft.CodeAnalysis.Common` so that it's easy to use it together with Roslyn.

Currently, the version of this library corresponds to the version of the referenced Roslyn NuGet package. However, the patch version might be increased independently if there are changes in the library itself while the referenced Roslyn version stays the same. For example, it might be useful to expose more embedded languages (JSON, etc.) in the future.
