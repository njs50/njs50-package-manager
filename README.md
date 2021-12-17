# njs50 package manager
package manager for TFE mudlet packages

## Exporting your catalog!
install the package manager with this command:
```
lua local a="https://raw.githubusercontent.com/njs50/njs50-package-manager/main/njs50-package-manager.xml"local b,c local d=function(e)cecho('\n<green>njs50pm: <white>package '..e..'\n')end b=registerAnonymousEventHandler("sysDownloadDone",function(f,g)if not g:find("njs50-package-manager.xml",1,true)then return end killAnonymousEventHandler(b)d('downloaded')installPackage(g)os.remove(g)end)c=registerAnonymousEventHandler("sysInstallPackage",function(f,h)if h~="njs50-package-manager"then return end killAnonymousEventHandler(c)d('installed')expandAlias('njs50-package-manager help')end)d('uninstalling any existing...')uninstallPackage('njs50-package-manager')tempTimer(5,function()d('downloading...')downloadFile(getMudletHomeDir().."/njs50-package-manager.xml",a..'?_='..tostring(getEpoch))end)
```


## developer info
feel free to fork this project. will prob need a recent node.js installed
