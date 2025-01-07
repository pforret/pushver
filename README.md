![bash_unit CI](https://github.com/pforret/pushver/workflows/bash_unit%20CI/badge.svg)
![Shellcheck CI](https://github.com/pforret/pushver/workflows/Shellcheck%20CI/badge.svg)
![GH Language](https://img.shields.io/github/languages/top/pforret/pushver)
![GH stars](https://img.shields.io/github/stars/pforret/pushver)
![GH tag](https://img.shields.io/github/v/tag/pforret/pushver)
![GH License](https://img.shields.io/github/license/pforret/pushver)
[![basher install](https://img.shields.io/badge/basher-install-white?logo=gnu-bash&style=flat)](https://www.basher.it/package/)

# pforret/pushver

![](assets/pushver.jpg)

Push new version of component into projects that use it

## 🔥 Usage

```
Program : pushver.sh  by peter@forret.com
Version : v0.0.1 (2024-12-27 17:27)
Purpose : Push new version of component into projects that use it
Usage   : pushver.sh [-h] [-Q] [-V] [-f] [-L <LOG_DIR>] [-T <TMP_DIR>] [-B <BRANCH>] <action> <component?> <application?>
Flags, options and parameters:
    -h|--help        : [flag] show usage [default: off]
    -Q|--QUIET       : [flag] no output [default: off]
    -V|--VERBOSE     : [flag] also show debug messages [default: off]
    -f|--FORCE       : [flag] do not ask for confirmation (always yes) [default: off]
    -L|--LOG_DIR <?> : [option] folder for log files   [default: /home/pforret/log/pushver]
    -T|--TMP_DIR <?> : [option] folder for temp files  [default: /tmp/pushver]
    -B|--BRANCH <?>  : [option] branch to update  [default: main]
    <action>         : [choice] action to perform  [options: php,check,env,update]
    <component>      : [parameter] component repo e.g. pforret/statistics_module (optional)
    <application>    : [parameter] application that uses the component and should be upgraded e.g. pforret/finixproject (optional)
                                                                                                                                                                                                                                                                                                                                                                 
### TIPS & EXAMPLES
* use pushver php to .push a new PHP component/library version into dependent applications (with composer)
  pushver php pforret/statistics_module pforret/finixproject
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
