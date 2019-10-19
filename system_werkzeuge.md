# Werkzeuge zur Systemkonfiguration
## Dateisystem
- lsof

### ACLs
- getfacl/setfacl

### Capabilities
- ???

## Namespaces
- lsns
- nsenter

## Prozesse
Alle Prozesse mit kompletter cmdline anzeigen:
  ps auxwww

Prozesse als Baum anzeigen:
  ps axjf
  pstree

## Weitere
Alternativen für editor anzeigen:
  update-alternatives --list editor

/usr/bin/vim.basic als Alternative für editor setzen:
  update-alternatives --set editor /usr/bin/vim.basic
