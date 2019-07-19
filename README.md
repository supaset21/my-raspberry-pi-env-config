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
