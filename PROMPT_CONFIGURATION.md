# Prompt Configuration for Warp Terminal

## Default Prompt
Warp has a native prompt that is customizable and can display various information, including:
- Current working directory (cwd)
- Git branch and uncommitted changes
- Subversion (SVN) information
- Kubernetes context
- Date and time

To customize the prompt:
1. Navigate to **Settings > Appearance > Prompt**.
2. Drag and drop context chips into your Warp prompt to display the desired information.

## Git and Subversion
- The Git context chip shows the current branch and the number of uncommitted changed files, including new, modified, and deleted files.
- The Subversion context chip provides similar information for SVN.

## Kubernetes
- The Kubernetes context chip displays relevant information when using commands like `kubectl`, `helm`, and others.
- Ensure the `KUBECONFIG` environmental variable is set to your preferred configuration file location if it's not the default path of `~/.kube/config`.

## Same Line Prompt
By default, Warp's prompt displays on two lines. To configure the prompt to display inline with the command line input:
1. Go to **Settings > Appearance > Prompt**.
2. Check the box for **Same line prompt**.

If using a custom prompt (PS1), Warp will respect the same line prompt settings.

### Adding New Line to Custom Prompt
To add a new line to your custom prompt, run the following commands based on your shell:

#### Bash
```bash
echo -e '\nPS1="${PS1}"$'\''\\n'\''' >> ~/.bashrc
```

#### Zsh
```bash
echo -e '\nPROMPT="${PROMPT}"$'\''\\n'\''' >> ~/.zshrc
```

#### Fish
```bash
echo -e '\nfunctions --copy fish_prompt fish_prompt_orig; function fish_prompt; fish_prompt_orig; echo; end' >> ~/.config/fish/config.fish
```

#### PowerShell
```powershell
$rawString = @'
$originalPrompt = Get-Item Function:\prompt
Set-Item -Path Function:\prompt_original -Value $originalPrompt
function prompt {
    "$(& prompt_original)`n"
}
'@
Add-Content -Path $PROFILE -Value "`n$rawString`n"
```

## Custom Prompt
You can set up a custom prompt by configuring the PS1 variable or installing a supported shell prompt plugin. The PS1 variable represents the primary prompt string displayed before typing new commands.

### Multi-Line and Right-Sided Prompts
Warp's custom prompt supports multi-line or right-sided prompts in zsh and fish, but not in bash. Note that you cannot have a multiline right-side prompt, only a multiline left prompt.

## Accessing the Custom Prompt
To toggle the custom prompt:
1. Right-click on the prompt area above the input and select **Edit prompt**.
2. Alternatively, select **Prompt** from the **Settings > Appearance** page.

When using Warp's prompt, you can right-click to copy the entire prompt or specific parts of the custom prompt from previously run blocks in your session.
