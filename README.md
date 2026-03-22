# Python Sample Code

## Preparation
1. install pyenv
- brew install pyenv
- Set up profile
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
echo 'eval "$(pyenv init -)"' >> ~/.bash_profile
source ~/.bash_profile
- install python and configure version to use (local is effective only for current folder)
pyenv install 3.8.0
pyenv local 3.7.0
pyenv global 3.8.0
pyenv list
python --version

[troubleshooting](https://github.com/pyenv/pyenv/wiki/Common-build-problems)
echo 'export LDFLAGS="-L/usr/local/opt/zlib/lib"' >> ~/.bash_profile
echo 'export CPPFLAGS="-I/usr/local/opt/zlib/include"' >> ~/.bash_profile
echo 'PKG_CONFIG_PATH="/usr/local/opt/zlib/lib/pkgconfig"' >> ~/.bash_profile

2. install venv
brew install venv
python3 -m venv venv

3. install direnv to activate venv automatically
brew install direnv
echo 'export EDITOR=vim' >> ~/.bashrc
echo 'eval "$(direnv hook bash)"' >> ~/.bashrc
source ~/.bashrc
echo 'source venv/bin/activate' > .envrc
direnv allow

## Tkinker

## Word/CSV

