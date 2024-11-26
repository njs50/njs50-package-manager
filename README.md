# njs50 package manager
package manager for TFE mudlet packages

## install the package manager
install the package manager by pasting this command into mudlet:
```
lua installPackage('https://tinyurl.com/ykjbnsf8/njs50-package-manager.xml')
```

## install a package
```
njs50pm install tfecat
```

## update all installed packages
```
njs50pm update
```

## developer info
feel free to fork this project and/or send pull requests

### creating a new module

copy empty-module.xml to modules/[new-module-name].xml

import the new module in mudlet and set to sync.
make changes / delete the placeholders etc.

commit the changes to a new branch, send me a pull request...
