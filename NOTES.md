autoload -U +X bashcompinit && bashcompinit
source /usr/local/etc/bash_completion.d/git-completion.bash

# for git autocompletion.
https://www.oliverspryn.com/blog/adding-git-completion-to-zsh

### install: 
- remmina remote desktop client
- virtual machine manager (or other)
- https://github.com/ryanoasis/nerd-fonts.git [install nerd-fonts: configure only the necessary]
https://medium.com/@akhilesh-mishra/terraform-documentation-made-easy-with-terraform-docs-096014b00ecf
- azure cli (also on the standard apps for ubuntu)

python3-pip install 

to only run a task or selected, need to tag the tasks like so:

- name: Copy .gitconfig file to home directory
      ansible.builtin.copy:
        src: "files/.gitconfig"
        dest: "{{ ansible_env.HOME }}/.gitconfig"
      tags: 
        - gitconfig

then run:
`ansible-playbook playbook.yaml --tags gitconfig`
or skip tasks:
`ansible-playbook playbook.yaml --skip-tags docker`


