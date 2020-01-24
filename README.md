# Powerob
An on-the-fly Powershell script obfuscator meant for red team engagements. Built out of necessity.

### Installation
`git clone https://github.com/cwolff411/powerob`

### Usage

`python3 powerob.py obfuscate originalfile.ps1 obfuscatedfile.ps1`

Takes an INPUTFILE obfuscates it and dumps the obfuscated version into OUTPUTFILE.

`python3 powerob.py list`

Lists all of the currently obfuscated files along with their commands and associated obfuscated commands.

`python3 powerob.py getcommand Invoke-AllChecks`

For reference on the fly for when you forget. Takes the original command name and displays the obfuscated command name to be used in Powershell.

`python3 powerob.py cleardb`

Maintenance function to clear the db of past obfuscated files and functions.

### About
This was built out of the need to bypass endpoint security on a recent engagement. During priv esc attempts I could not download [PowerUp.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Privesc/PowerUp.ps1) until it was obfuscated.

This is v1. It obfuscates the functions only and I will enhance the functionality as time allows. Pull requests and collaboration welcomed.

I work at [Layer 8 Security](https://layer8security.com). Come say hi.

### License
[MIT License](https://opensource.org/licenses/MIT)