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


Cow say
```
# Cowsay
arr[0]=default
arr[1]=tux
arr[2]=sheep
arr[3]=bud-frogs
BOOL=$[RANDOM %${#arr[*]}]
fortune | cowsay -f ${arr[$BOOL]}

# History
HISTCONTROL=ignorespace
HISTTIMEFORMAT="%F %T  "
```  


starship
```
curl -fsSL https://starship.rs/install.sh | bash

echo '# starship' >> /home/jorge/.bashrc
echo 'eval "$(starship init bash)"' >> /home/jorge/.bashrc
```

fzf
```
echo '# fzd' >> /home/jorge/.bashrc
echo '/usr/share/fzf/shell/key-bindings.bash' >> /home/jorge/.bashrc
echo '/etc/bash_completion.d/fzf' >> /home/jorge/.bashrc
```
