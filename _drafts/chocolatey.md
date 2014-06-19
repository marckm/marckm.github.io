
------------------------------
Chocolatey install:

get install.ps1 source from web
add following lines to make proxy work


# specify your proxy address and port
$proxy = new-object System.Net.WebProxy "proxy:8080"
# Getting credentials for proxy Authentication
$proxy.Credentials = Get-Credential
$downloader.proxy=$proxy

Save on desktop
Start with cmd:

@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ./install.ps1" && SET PATH=%PATH%;%systemdrive%\chocolatey\bin



note: how to update all: cup all


------------------------------
software installed using Chocolatey:

cinst 7zip.install
cinst fiddler
cinst filezilla
cinst paint.net
cinst linqpad4
cinst winmerge
