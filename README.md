# Config

This is my basic config raspberry pi

# Install Vscode

[ตัวอย่าง](https://medium.com/@iSnoopy/%E0%B8%A1%E0%B8%B2%E0%B8%95%E0%B8%B4%E0%B8%94%E0%B8%95%E0%B8%B1%E0%B9%89%E0%B8%87-visual-studio-code-%E0%B8%9A%E0%B8%99-raspberry-pi-%E0%B8%81%E0%B8%B1%E0%B8%99%E0%B9%80%E0%B8%96%E0%B8%AD%E0%B8%B0-49e8890f4fe1)

`curl -s https://packagecloud.io/install/repositories/headmelted/codebuilds/script.deb.sh | sudo bash`

`sudo apt-get install code-oss`

If doesn't success show below command

`error unable to locate package`

edit `stretch` or `bluster` in file `headmelted_codebuilds.list` to `jessie`

Use this command

`sudo nano /etc/apt/sources.list.d/headmelted_codebuilds.list`

After do this run command

```command
sudo apt-get update
sudo apt-get install code-oss
```

# Install pyenv for raspberry pi

[ตัวอย่าง](http://www.knight-of-pi.org/pyenv-for-python-version-management-on-raspbian-stretch/)

run below command
```
sudo apt-get install bzip2 libbz2-dev libreadline6 libreadline6-dev libffi-dev libssl1.0-dev sqlite3 libsqlite3-dev -y
git clone git://github.com/yyuu/pyenv.git .pyenv
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init -)"' >> ~/.bashrc
. ~/.bashrc
```

pyenv install example
```
pyenv install 3.6.3
```

pyenv check version
```
pyenv versions
```

change global version
```
pyenv global 3.6.3
```

after change don't forgot refresh command
```
exec -l $SHELL
```
