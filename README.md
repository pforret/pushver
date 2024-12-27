![bash_unit CI](https://github.com/pforret/pushver/workflows/bash_unit%20CI/badge.svg)
![Shellcheck CI](https://github.com/pforret/pushver/workflows/Shellcheck%20CI/badge.svg)
![GH Language](https://img.shields.io/github/languages/top/pforret/pushver)
![GH stars](https://img.shields.io/github/stars/pforret/pushver)
![GH tag](https://img.shields.io/github/v/tag/pforret/pushver)
![GH License](https://img.shields.io/github/license/pforret/pushver)
[![basher install](https://img.shields.io/badge/basher-install-white?logo=gnu-bash&style=flat)](https://www.basher.it/package/)

# pushver

![](assets/pushver.jpg)

Push new version of component into projects that use it

## 🔥 Usage

```
Program : pushver  by peter@forret.com
Version : v0.0.1 (Apr 22 16:07:13 2023)
Purpose : Push new version of component into projects that use it
Usage   : pushver [-h] [-q] [-v] [-f] [-l <log_dir>] [-t <tmp_dir>] <action>
Flags, options and parameters:
    -h|--help        : [flag] show usage [default: off]
    -q|--quiet       : [flag] no output [default: off]
    -v|--verbose     : [flag] also show debug messages [default: off]
    -f|--force       : [flag] do not ask for confirmation (always yes) [default: off]
    -l|--log_dir <?> : [option] folder for log files   [default: /Users/pforret/log/script]
    -t|--tmp_dir <?> : [option] folder for temp files  [default: /tmp/script]
    <action>         : [choice] action to perform  [options: action1,action2,check,env,update]
                                  
### TIPS & EXAMPLES
* use pushver action1 to ...
  pushver action1
* use pushver action2 to ...
  pushver action2
* use pushver check to check if this script is ready to execute and what values the options/flags are
  pushver check
* use pushver env to generate an example .env file
  pushver env > .env
* use pushver update to update to the latest version
  pushver update
* >>> bash script created with pforret/bashew
* >>> for bash development, also check out pforret/setver and pforret/progressbar
```

## ⚡️ Examples

```bash
> pushver -h 
# get extended usage info
> pushver env > .env
# create a .env file with default values
```

## 🚀 Installation

with [basher](https://github.com/basherpm/basher)

	$ basher install pforret/pushver

or with `git`

	$ git clone https://github.com/pforret/pushver.git
	$ cd pushver

## 📝 Acknowledgements

* script created with [bashew](https://github.com/pforret/bashew)

&copy; 2024 pforret
