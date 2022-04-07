# Remote Desktop

## Download Cloudflare Tunnel

Download [Cloudflared for Windows 64-bit](https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-amd64.exe)

## Start tunnel

```PowerShell
cloudflared.exe access rdp --hostname rdp.seccore.com --url localhost:3390
```

## Connect to Remote Desktop

```PowerShell
mstsc.exe /v:localhost:3390 /f
```

## Shortcut

```PowerShell
C:\Windows\System32\cmd.exe /k "start C:\Windows\System32\cloudflared.exe access rdp --hostname rdp.seccore.com --url localhost:3390 && mstsc /v:localhost:3390 /f"
```
