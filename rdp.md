# Remote Desktop

Download [Cloudflared for Windows 64-bit](https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-amd64.exe)

## Tunnel
<code>cloudflared.exe access rdp --hostname rdp.seccore.com --url localhost:3390</code>

## Remote Destop Connection
<code>mstsc.exe /v:localhost:3390 /f</code>

## Shortcut

<code>
C:\Windows\System32\cmd.exe /k "start C:\Windows\System32\cloudflared.exe access rdp --hostname rdp.seccore.com --url localhost:3390 && mstsc /v:localhost:3390 /f"
</code>