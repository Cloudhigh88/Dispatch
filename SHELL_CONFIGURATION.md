# Shell Configuration for Warp Terminal

## Supported Shells
Warp supports the following shells across macOS, Windows, and Linux:
- **macOS and Linux**: bash, zsh, fish, PowerShell (pwsh)
- **Windows**: PowerShell 5 & 7, WSL2, Git Bash

## Default Shells
- **macOS**: zsh is the default shell.
- **Windows**: PowerShell (pwsh) is the default shell.
- **Linux**: bash is the default shell.

## Changing the Default Shell
To change the default shell in Warp:
1. Go to **Settings > Features**.
2. Scroll to the **Session** section.
3. Select the desired shell under "Startup shell for new sessions".

## Customizing Your Shell Environment

### Zsh
- **Configuration File**: `~/.zshrc`
- **Editing**: Use `nano ~/.zshrc` or `vi ~/.zshrc`.
- **Reloading**: Run `source ~/.zshrc` or restart Warp.

### Bash
- **Configuration Files**: `~/.bashrc` (non-login shells) or `~/.bash_profile` (login shells).
- **Editing**: Use `nano ~/.bashrc` or `vi ~/.bashrc`.
- **Reloading**: Run `source ~/.bashrc` or restart Warp.

### Fish
- **Configuration File**: `~/.config/fish/config.fish`
- **Editing**: Use `nano ~/.config/fish/config.fish`.
- **Reloading**: Run `source ~/.config/fish` or restart Warp.

### PowerShell (pwsh)
- **Profile Script**: `$PROFILE`
- **Editing**: Use `code $PROFILE`.
- **Reloading**: Restart Warp or open a new session.
- **Execution Policy**: Enable profile execution with:
  ```powershell
  Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```

## Additional Shell Guidance for macOS
### Setting Up Zsh
- Confirm location: `which zsh`
- Check version: `zsh --version`

### Using Fish Shell
1. **Install Fish**: `brew install fish`
2. **Set as Default Shell**:
   ```bash
   echo $(which fish) | sudo tee -a /etc/shells
   chsh -s $(which fish)
   ```

### Using PowerShell (pwsh)
1. **Install PowerShell**: `brew install powershell/tap/powershell`
2. **Set as Default Shell**:
   ```bash
   echo $(which pwsh) | sudo tee -a /etc/shells
   chsh -s $(which pwsh)
   ```

## Using Warp with Shells on Windows
- **Default Shell**: PowerShell 7 (pwsh).
- **Supported Shells**: PowerShell 5, WSL2, Git Bash.
