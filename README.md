# DevOps Macbook Machine
- This playbook installs most of the tools needed for DevOps and configure your Macbook accordingly.

`Work in progress: need to install more tools`

_NOTE ON INSTALLING ANSIBLE and the right PERMISIONS_

```bash
$ cd ~
$ find . | grep ansible | more
<lines omitted>
./Library/Python/3.9/bin/ansible
<lines omitted>

# From there, its pretty easy, just update your .bash_profile or .zshrc with

export PATH="/path/to/Library/Python/3.8/bin:$PATH"

$ source ~/.zshrc
$ ansible --version
ansible 2.10.8
  config file = None
  configured module search path = ['/Users/dbove/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
```
## Check the ownership of ~/.ansible directory:
`ls -l ~/.ansible` => adjust to your user if needed. (ansible should run WITHOUT sudo)
