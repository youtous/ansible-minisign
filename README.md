# youtous/ansible-minisign

[![pipeline status](https://gitlab.com/youtous/ansible-minisign/badges/master/pipeline.svg)](https://gitlab.com/youtous/ansible-minisign/-/commits/master)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![GitHub Repo stars](https://img.shields.io/github/stars/youtous/ansible-minisign?label=✨%20youtous%2Fansible-minisign&style=social)](https://github.com/youtous/ansible-minisign/)
[![Gitlab Repo](https://img.shields.io/badge/gitlab.com%2Fyoutous%2Fansible--minisign?label=✨%20youtous%2Fansible-minisign&style=social&logo=gitlab)](https://gitlab.com/youtous/ansible-minisign/)
[![Licence](https://img.shields.io/github/license/youtous/ansible-minisign)](https://github.com/youtous/ansible-minisign/blob/master/LICENSE)


This ansible role permits to easily install or update [minisign](https://jedisct1.github.io/minisign/) on debian like OS.

Installation from [ansible galaxy](https://galaxy.ansible.com/youtous/minisign): `ansible-galaxy install youtous.minisign`

```yaml
- name: Install minisign
  ansible.builtin.include_role: youtous.minisign
  vars:
    minisign_version: "0.10" # optional
```

### Requirements

- ansible-core 2.11+

### Usage

```yaml
minisign_version: '0.10'

# sha512sum of the minisign archive, optional when minisign is already installed on the system
# get it using:
# $ minisign -Vm minisign-0.10.tar.gz -P 'RWQf6LRCGA9i53mlYecO4IzT51TGPpvWucNSCh1CBM0QTaLn73Y7GFO3' && sha512sum minisign-0.10.tar.gz
minisign_version_sha512sum: 'dae9eb52888affd040da832820a5c9e236bbd3f4d320a29868cf85bfadd923b755eb736838c85fb93adac27168cbe856a1a3abdfb984d015b145df0e03df5b73'

```

### License

MIT
