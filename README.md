# Cisco Facts and Genie Parsed Commands to Business-Ready Documentation Ansible Playbooks

[![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/automateyournetwork/Cisco_Facts)

## Written by John Capobianco

Ansible has several "Facts" modules - ios_facts and nxos_facts - that capture data and transform it into JavaScript Object Notation (JSON) which we then use Jinja2 Templates to transform again into business-ready documentation

Cisco also has release Genie parsers - combined with Ansible you can first run an IOS / NXOS show command, then with Genie, parse that command into JSON. Once you have the JSON you can transform it with Jinja2 into CSV / MD! 

### Prerequisites

1) Install Ansible
```console
pip install --user ansible
```

2) Check version of Ansible
```console
ansible --version

ansible 2.9.1
```

3) Install JMESPATH
```console
pip install --user jmespath
```

4) Install Genie 
```console
pip install genie
```

5) Install node.js 12
```console
curl -sL https://rpm.nodesource.com/setup_12.x | sudo bash -
```
6) Install GCC
```console
sudo yum install -y gcc-c++ make
```

7) Install Node.js  
```console
sudo yum install -y nodejs
```

8) Install Mark Map
```console
npm install markmap-lib -g  
```
9) Clone the Repository
```console
git clone https://github.com/automateyournetwork/Cisco_Facts
```
### IOS and NXOS Facts

0) Update your hosts to match your CAMPUS or DC first. Make sure you have SSH connectivity from the Ansible host.

1) Run the ansible-playbook of choice

2) Supply Username

3) Supply Secret

4) Git add / commit / push created output files

5) Check output .CSV files

6) Check output .MD files

7) Check output .HTML files
