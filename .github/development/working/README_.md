[🏠︎](README.md) ❭ Applications > Visual Studio 2026

<div align="center">

### The Documentation Project

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../../.github/logo/light/256x256.png">
  </picture>

# Visual Studio 2026

</div>

| CONTENTS |
| -------- |
| [Setup](#setup) |
| [Extensions](#extensions) |
| [Configure](#configure) |
| [Publishing](#publishing) |





## Publishing

How to publish as a single file:

1. Right-click on the project you want to publish, and choose "Publish"
2. Click "Add a publish profile"
3. For the Target, choose "Folder"
4. Choose the Specific target, choose "Folder"
5. Choose a folder location to publish to.

For example:

`release\`

6. Click "Close"
7. Click "Show all settings"

WPF projects should look like this:

![](./Resources/readme-01.png)

Console projects should look like this:

![](./readme-02.png)

8. Click "Save".

9. Add the following to the .csproj file:

```csharp
<PropertyGroup>
    <DebugType>embedded</DebugType>
    <IncludeAllContentForSelfExtract>true</IncludeAllContentForSelfExtract>
    <Version>1.0.0</Version>
    <FileVersion>1.0.0</FileVersion>
</PropertyGroup>
```

### Multi-project solutions

If a solution has multiple projects, each project needs to be published.

# More

https://learn.microsoft.com/en-us/dotnet/core/deploying/

***

[🏠︎](README.md) ❭ Applications > Visual Studio 2026

<sub>Last updated: 260713</sub>
