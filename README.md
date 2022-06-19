# youtous/ansible-minisign

This ansible role permits to easily install or update [minisign](https://jedisct1.github.io/minisign/) on debian like OS.

Installation from [ansible galaxy](https://galaxy.ansible.com/youtous/minisign): `ansible-galaxy install youtous.minisign`

```yaml
- name: Install minisign
  include_role: youtous.minisign
  vars:
    minisign_version: "0.10" # optional
```

### Usage

```yaml
minisign_version: '0.10'

# sha512sum of the minisign archive, optional when minisign is already installed on the system
# get it using:
# $ minisign -Vm minisign-0.10.tar.gz -P 'RWQf6LRCGA9i53mlYecO4IzT51TGPpvWucNSCh1CBM0QTaLn73Y7GFO3' && sha512sum minisign-0.10.tar.gz
minisign_version_sha512sum: 'dae9eb52888affd040da832820a5c9e236bbd3f4d320a29868cf85bfadd923b755eb736838c85fb93adac27168cbe856a1a3abdfb984d015b145df0e03df5b73'

```

### Licence
MIT