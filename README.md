# INSALAN - dockcsgo

This project is the configuration (and deployment tool) of the InsaLan's CSGO servers. Look and adapt your configuration in the start.py file to your needs. All images need to be made beforehand.

## Usage
When your configuration is accurate and your images are built, simply use this command : python3 start.py

## Dependencies
- docker
- ipaddress
- mysql-connector-python
you just need to run pip install -r requirements.txt to install all dependencies

## FAQ
- server token ? tokens=["youtoken"] in key.py
- Csgo server outdated ? docker rmi csgoserver && make build
- python script not working ? either you broke it, or you are not using the venv
- passwords ? find . -type f -exec grep --color -n -e password /dev/null \{\} +
- how to setup servers array ? simply add your servers with the following syntax : {'ip': 'xxx.xxx.xxx.xxx'}
- macvlan or host ? use macvlan at your own risks