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

	a. Edit
	
		```bash
		
			nano ~/.zshrc
			
		```
		
		_change theme settings line to **PowerLevel10K**_
		
		```bash
		
			ZSH_THEME="powerlevel10k/powerlevel10k"
			
		```
	b. Reload .zshrc