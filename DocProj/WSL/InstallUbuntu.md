<!-- 260501 -->

[The Documentation Project](../README.md) ❭ WSL ❭ Install a WSL Ubuntu distribution

***

<div align="center">

<h1>Install a WSL Ubuntu distribution</h1>
ee
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../.github/logo/light/256x256.png">
  </picture>

</div>

1. Install WSL. By default, this will also install Ubuntu.

```bash
$ wsl --install
```

2. Create a user account and password.

3. Move the WSL distribution to a different drive.
```bash
$ wsl --shutdown Ubuntu
$ wsl --manage Ubuntu --move B:\wsl
```

4. Update the Ubuntu distribution.

```bash
sudo apt update && sudo apt upgrade
```

5. Export the Ubuntu distribution to backup.

> [!NOTE]
> The .vhdx will be exported to your user folder.

```bash
wsl --export Ubuntu Wsl-Ubuntu-Base-YYMMDD.vhdx --vhd
```

<br>

***

[The Documentation Project](../README.md) ❭ WSL ❭ Install a WSL Ubuntu distribution
