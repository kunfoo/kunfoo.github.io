# Paketmanager

## apt/dpkg
- `apt-file search $FILE`
- `dpkg -S $FILE`

## yum/dnf/rpm
- `yum whatprovides $FILE`
  - search for packet which installs $FILE
- `rpm -qf $FILE`
  - tell which packet installed $FILE
