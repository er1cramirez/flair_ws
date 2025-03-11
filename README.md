# flair_ws
## Setup
```
mkdir $HOME/flair
```
### Include in .bashrc
```
# variable for Flair
export FLAIR_ROOT=$HOME/flair
# flair binaries
export PATH="$PATH":"$FLAIR_ROOT"/flair-src/bin
# flair completion script
source "$FLAIR_ROOT"/flair-src/scripts/flair_completion.sh 
```

### Pre
```
sudo apt update && upgrade
```
```
sudo apt install python
sudo apt install g++
sudo apt install mesa-utils libgl1-mesa-dev
```

### Install toolchains

```
wget https://devel.hds.utc.fr/flair/old/toolchain/x86_64-meta-toolchain-flair-x86_64.sh
chmod +x x86_64-meta-toolchain-flair-x86_64.sh
sudo -E ./x86_64-meta-toolchain-flair-x86_64.sh
rm x86_64-meta-toolchain-flair-x86_64.sh
source ~/.bashrc
```
