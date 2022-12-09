<img align="center" width="800" src="ITerm2 + OhMyZsh + P10K.png">


# 1. Install Oh My Zsh - (Custom Terminal Prompts)
> https://github.com/ohmyzsh/ohmyzsh/
```bash
	sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
# 2. Download - Oh My Zsh - Theme - PowerLevel10K
> https://github.com/romkatv/powerlevel10k

```bash
	git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

# 3. Install Required Fonts
> https://github.com/romkatv/powerlevel10k-media

- MesloLGS NF Regular.ttf
- MesloLGS NF Bold.ttf
- MesloLGS NF Italic.ttf
- MesloLGS NF Bold Italic.ttf

_Files will download to your Home Directory / Downloads Folder_
    
```bash
	curl -fsSL https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf --output ~/Downloads/MesloLGS\ NF\ Regular.ttf
```
```bash
	curl -fsSL https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf --output ~/Downloads/MesloLGS\ NF\ Bold.ttf
```
```bash
	curl -fsSL https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf --output ~/Downloads/MesloLGS\ NF\ Italic.ttf
```
```bash
	curl -fsSL https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf --output ~/Downloads/MesloLGS\ NF\ Bold\ Italic.ttf
```

# 4. Your Favorite Terminal - Load Theme - Edit [.zshrc](https://toolspond.com/zshrc/)
### a. Edit
	
```bash
		
	nano ~/.zshrc
			
```
		
## Change theme settings line to **PowerLevel10K**
		
```bash
		
	ZSH_THEME="powerlevel10k/powerlevel10k"
			
```

## _PATH_

### b. Uncomment Path Export
> OhMyZsh backups your former .zshrc so make sure to copy your old custom PATH.
> Old zshrc file name is:

```bash
	.zshrc.pre-oh-my-zsh
```

#### c. Reload .zshrc
```bash
	source ~/.zshrc
```
# 5. Run PowerLevel10K Settings
```bash
	p10k configure
```

# 6. Your Favorite Terminal - Font Size & Colors
> _iTerm2's "Smoooth" Color Preset is nice_