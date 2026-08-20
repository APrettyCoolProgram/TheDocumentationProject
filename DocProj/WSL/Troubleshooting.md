<!-- 260501 -->

[The Documentation Project](../README.md) ❭ WSL ❭ Troubleshooting WSL

***

<div align="center">

<h1>Troubleshooting WSL</h1>

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../.github/logo/light/256x256.png">
  </picture>

</div>

## Try restarting the `VSCompute` service

```bash
Get-Service vmcompute | Restart-Service -force
```

## Try uninstalling/reinstalling WSL

```bash
$ dism.exe /online /disable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
$ wsl --uninstall
```

Reboot the machine

```bash
$wsl --install
```

<br>

***

[The Documentation Project](../README.md) ❭ WSL ❭ Troubleshooting WSL
