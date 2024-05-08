## Install Ansible
```
sudo dnf install -y ansible
```

## Copy applications to files directory

## Run playbook

Fedora 31

```sh
ansible-playbook fedora31.yml
```

Fedora 32
```sh
ansible-galaxy collection install ansible.posix
ansible-playbook --ask-become-pass fedora32.yml
```

Fedora 34
```sh
ansible-galaxy collection install ansible.posix
ansible-playbook --ask-become-pass fedora34.yml
```

Fedora 36
```sh
ansible-playbook --ask-become-pass fedora36.yml
```

Fedora 38
```sh
ansible-galaxy collection install community.general
ansible-galaxy collection install ansible.posix
ansible-playbook --ask-become-pass fedora38.yml
```

Fedora 40
```sh
ansible-playbook --ask-become-pass fedora40.yml
```

.bashrc
```
# Cowsay
arr[0]=default
arr[1]=tux
arr[2]=sheep
arr[3]=bud-frogs
BOOL=$[RANDOM %${#arr[*]}]
fortune | cowsay -f ${arr[$BOOL]}

# History
HISTCONTROL=ignorespace:ignoredups
HISTTIMEFORMAT="%F %T  "
HISTSIZE=20000
HISTFILESIZE=20000
```  


starship
```
curl -sS https://starship.rs/install.sh | sh

echo '# starship' >> /home/jorge/.bashrc
echo 'eval "$(starship init bash)"' >> /home/jorge/.bashrc
```

fzf
```
echo '# fzd' >> /home/jorge/.bashrc
echo '[ -f /usr/share/fzf/shell/key-bindings.bash ] && source /usr/share/fzf/shell/key-bindings.bash' >> /home/jorge/.bashrc
```
