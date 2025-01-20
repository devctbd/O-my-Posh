# O-my-Posh

<h2>Beautiful Terminal on Windows using Oh-My-Posh</h2>

<img src="https://i.ibb.co.com/7t76qDP/New-Project.png" />

<p>Terminal is the most important part of the Windows experience. It is the place where you spend most of your time. It is the place where you spend most of your time.</p>

<h2> Open Termianl </h2>

```
Set-ExecutionPolicy -ExecutionPolicy Unrestricted

```

<h3>Installation</h3>

```
powershell

winget install JanDeDobbeleer.OhMyPosh -s winget

```

<h3> After installation, type in the terminal</h3>

```

notepad $PROFILE

```

<h3> If this shows profile not found error, type this command</h3>

```
New-Item -Path $PROFILE -Type File -Force

```

<h2> Then re-run this command again:</h2>

```
oh-my-posh init pwsh --config 'C:\Users\< dextop username>\AppData\Local\Programs\oh-my-posh\themes\craver.omp.json' | Invoke-Expression

```

<h3> For autocomplete, we have to install a module.</h3>

```
Install-Module PSReadLine -Force

```

<h3>After installation is complete, go to the PowerShell config file again and paste these lines:</h3>

```
Import-Module PSReadLine
Set-PSReadLineOption -EditMode Windows
Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle ListView
Set-PSReadLineOption -PredictionViewStyle InlineView

```
