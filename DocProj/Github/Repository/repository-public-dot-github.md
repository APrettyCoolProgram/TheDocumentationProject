<!-- 260331 -->

[The Documentation Project](../README.md) ❭ Repository ❭ The public .github repository

***

<div align="center">

### The APCP Documentation Project

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../../.github/logo/light/256x256.png">
  </picture>

# The public `.github` repository

</div>

The public `.github` repository is a place to store resources that all individual repositories can access.

> [!NOTE]
> You can download a public .github folder template [here](../templates/PublicDotGithubRepository.7z).

## Examples of public `.github` repository files

Examples of files that you might want in the public `.github` repository are:

- CONTRIBUTING.md
- CODE_OF_CONDUCT.md
- SECURITY.md
- Issue and Pull Request templates
- Etc.

## About files in the public `.github` repository

Files in the public `.github` repository:

- Are used when an individual repository does not have the file  
  For example, the `CONTRIBUTING.md` file exists in the public `.github` repository, but not the repository `.github/` folder

- Won’t appear in the file browser or `.git` history of individual repositories

- Aren’t included in clones, packages, or downloads

## Order of precedence

The order of precedence looks like this:

The **public `.github` repository** → the **repository `.github/` folder** → the **repository root** → the **repository `docs/` folder**

> [!TIP]
> Thom Hayner has a nice writeup about [the .github/ Folder](https://thomhayner.com/blog/2024-02-01/dot-github-the-folder/).

# Creating files

To create a file that is accessible by individual repositories:

1. Create a *public* repository named `.github`
2. Create a `.github/` folder in the `.github` repository
3. Add the file to the `.github/` folder

## Typical `.github` repository files:

```text
\---.github
    |   CODEOWNERS
    |   CODE_OF_CONDUCT.md
    |   CONTRIBUTING.md
    |   README.md
    |   SECURITY.md
    |   SUPPORT.md
    |   
    +---ISSUE_TEMPLATE
    |       bug_report.yml
    |       documentation_request.yml
    |       feature_request.yml
    |       question.yml
    |       
    +---Profile
    |       README.md
    |       
    \---PULL_REQUEST_TEMPLATE
            PULL_REQUEST_TEMPLATE.md
```

> [!NOTE]
> For additional details, including the types of file you can add to the `.github/` folder, please see [Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

<br>

***

[The Documentation Project](../README.md) ❭ Repository ❭ The public .github repository
