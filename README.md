<p align="center"><b>PACSTALL</b></p>
<p align="center">
<a href="https://github.com/pacstall/pacstall"><img align="center" src="https://pacstall.dev/image/pacstall.svg" alt="Pacstall Logo"></a>
</p>
<p align="center"><b>The AUR Ubuntu never had</b></p>

<p align="center">Pacstall will attempt to become the AUR Ubuntu wishes it had. It takes the AUR and puts a spin on it, making it easier to install programs without scouring github repos and the likes</p>
</p>

---

### Installing

You can run the command below to install Pacstall.
```bash
sudo bash -c "$(curl -fsSL https://git.io/JsADh || wget -q https://git.io/JsADh -O -)" && sudo pacstall -A https://github.com/cutefishos-ubuntu/cutefish-pacstall
```
---

### Basic Commands
This will install foo. Equivalent of apt install
```bash
sudo pacstall -I foo
``` 

This will remove foo. Equivalent of apt remove
```bash
sudo pacstall -R foo
```

This will search for foo in repositories. Equivalent of apt search
```bash
sudo pacstall -S foo
```

Run this command with a github/gitlab url to add a repo
```bash
sudo pacstall -A
```

This will update pacstall's scripts
```bash
sudo pacstall -U
```

This will update packages. Equivalent of apt upgrade
```bash
sudo pacstall -Up
```

These are the basic commands, for more info, run `pacstall -h`

---
### Auto completions
Pacstall has fully supported auto completions for the `bash`, and `fish` shells. For the `ZSH` shell you can emulate the completions using the following commands.
#### Zsh auto completion
Zsh can emulate bash completion scripts by default so all you have to do is add these to your `.zshrc` or wherever you source things:
```bash
autoload bashcompinit
bashcompinit
source /usr/share/bash-completion/completions/pacstall
```

### License
---
![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)
```monospace
Pacstall is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, version 3 of the License

Pacstall is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Pacstall. If not, see <https://www.gnu.org/licenses/>.
```
