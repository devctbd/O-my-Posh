<h2>Beautiful Terminal on Windows using Oh-My-Posh</h2>

<img src="https://i.ibb.co/7t76qDP/New-Project.png" />

<p>Terminal is the most important part of the Windows experience. It is the place where you spend most of your time. It is the place where you spend most of your time.</p>

<h2> Installation </h2>

<ol>
  <li>
    <p>Open terminal.</p>
    <pre><code>Set-ExecutionPolicy -ExecutionPolicy Unrestricted</code></pre>
  </li>
  <li>
    <p>Install <code>Oh-My-Posh</code>.</p>
    <pre><code>winget install JanDeDobbeleer.OhMyPosh -s winget</code></pre>
  </li>
  <li>
    <p>Edit your PowerShell profile.</p>
    <pre><code>notepad $PROFILE</code></pre>
  </li>
  <li>
    <p>If the previous step shows a "profile not found" error, run this command.</p>
    <pre><code>New-Item -Path $PROFILE -Type File -Force</code></pre>
  </li>
  <li>
    <p>Initialize Oh-My-Posh.</p>
    <pre><code>oh-my-posh init pwsh --config 'C:\Users\< dextop username>\AppData\Local\Programs\oh-my-posh\themes\craver.omp.json' | Invoke-Expression</code></pre>
  </li>
</ol>

<h3> For autocomplete, we have to install a module.</h3>

<pre><code>Install-Module PSReadLine -Force</code></pre>

<h3>After installation is complete, go to the PowerShell config file again and paste these lines:</h3>

<pre><code>Import-Module PSReadLine
Set-PSReadLineOption -EditMode Windows
Set-PSReadLineOption -PredictionSource History
Set-PSReadLineOption -PredictionViewStyle ListView
Set-PSReadLineOption -PredictionViewStyle InlineView</code></pre>

<ol>
  <li>
  <h2> Font install </h2>

<pre><code>scoop bucket add nerd-fonts</code></pre>

  </li>
  <li>
  <h2>Again install the font</h2>

<pre><code>scoop install Cascadia-Code</code></pre>
  </li>
 </ol>

<ol>
<li>
<h3>Vs code terminla font setup.</h3>

<pre><code>"terminal.integrated.fontFamily": "Cascadia Code NF",</code></pre>
</li>
</ol>
