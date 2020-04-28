# youtous/ansible-minisign

This ansible role permits to easily install or update [minisign](https://jedisct1.github.io/minisign/) on debian like OS.

Installation from [ansible galaxy](https://galaxy.ansible.com/youtous/minisign): `ansible-galaxy install youtous.minisign`

```yaml
- name: Install minisign
  include_role: youtous.minisign
  vars:
    minisign_version: "0.8" # optional
```

### Usage

```yaml
minisign_version: '0.8'

# sha512sum of the minisign archive, optional when minisign is already installed on the system
# get it using:
# $ minisign -Vm minisign-0.8.tar.gz -P 'RWQf6LRCGA9i53mlYecO4IzT51TGPpvWucNSCh1CBM0QTaLn73Y7GFO3' && sha512sum minisign-0.8.tar.gz
minisign_version_sha512sum: '79bf626d0c15e39ce3bdf53600038028c0b22904b648074bf516a9ea6962c9486c41244e80637a5fbac090cce1ed9b4b3d57b8a02632646e01b43aa413cd8bd9'

```

### Licence
MIT