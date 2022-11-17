# citrix_adc

### Installing Pre-requisites
---
#### Install `ansible`
Run the below commands to install ansible:
```bash
python -m pip install --upgrade pip
python -m pip install ansible==5.5.0
```
After installing, you can verify if the installation is successful by the below command.
```bash
ansible --version
```

#### Install `Citrix ADC Python SDK`
In this, we will install the `Citrix ADC Python SDK` to use `ansible` to configure `citrix adc` devices.

First, clone our `citrix-adc-ansible-modules` github repo
```bash
git clone https://github.com/citrix/citrix-adc-ansible-modules.git /tmp/citrix-adc-ansible-modules
```

Then, run the below command to install the `Citrix ADC Python SDK`.
```bash
pip install /tmp/citrix-adc-ansible-modules/deps/nitro-python-1.0_kamet.tar.gz
```

#### Install `Citrix ADC Ansible Modules`
Next, we will install citrix-adc ansible modules from ansible-galaxy hub by running the below command.
```bash
ansible-galaxy collection install git+https://github.com/citrix/citrix-adc-ansible-modules.git#/ansible-collections/adc
```
---

#### Ansible Galaxy Offline Install
```bash
ansible-galaxy collection install xxxx.tar.gz
```
