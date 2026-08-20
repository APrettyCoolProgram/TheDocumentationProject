<!-- Last updated: 260820 -->

❰ [Back to The Documentation Project](./../../README.md)

<div align="center">

  <img src="./../../.github/logo/DocProj-478x116.png" alt="The Documentation Project">

  <br/>

 <h1>ProjectInfo file</h1>

</div>

Each project should have a `ProjectInfo` file with XML Documentation (or equivalent) containing the following information about the project:

* A detailed description of the project
* Information about project resources (repositories, websites, etc.)
* Project documentation

The XML documentation can either be in the source code, or in an external file.

## ProjectInfo.cs

A C# project would have a `ProjectInfo.cs` file with the following content:

```csharp
// =============================================================================
// %ProjectName%
// %ProjectDescription%
// %ProjectURL%
// Copyright (c) A Pretty Cool Program. All rights reserved.
// Licensed under the Apache 2.0 license.
// =============================================================================

// v0.0.0.0

namespace %Namespace%;

    internal class ProjectInfo
    {
        // This class is only used for informational purposes, and does not contain executable code.
    }
```

For example:

```csharp
// =============================================================================
// dvn
// A command line utility for managing development environments.
// https://github.com/APrettyCoolProgram/dvn
// Copyright (c) A Pretty Cool Program. All rights reserved.
// Licensed under the Apache 2.0 license.
// =============================================================================

// Version 1.0.1 (Build 250802)


namespace dvn;

    internal class ProjectInfo
    {
        // This class is only used for informational purposes, and does not contain executable code.
    }
```

<br>

***

❰ [Back to The Documentation Project](./../../README.md)