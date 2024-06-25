# oh-my-posh-custom-theme
Custom theme written for "oh-my-posh" plugin for windows power shell

## Create Customized Theme
* Ref 1 : https://ohmyposh.dev/docs/configuration/general
* Ref 2 : https://ohmyposh.dev/docs/installation/customize

## Add your customized Theme file in below location:

Note: Install oh-my-posh before steps below.

Put the customized JSON themes file under the below folder. Refer to this "quick-term-customized-plus.omp.json" for customized theme.

Folder Locaton: C:\Users\...\AppData\Local\Programs\oh-my-posh\themes


## Apply your themes (Ref: https://ohmyposh.dev/docs/installation/prompt)

notepad $PROFILE

# Sample PROFILE content:

oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\quick-term-customized-plus.omp.json" | Invoke-Expression

Import-Module -Name Terminal-Icons
Import-Module -Name PSReadLine

Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle ListView
Set-PSReadLineOption -EditMode Windows
