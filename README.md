

# WORK IN PROGRESS!!


## Install Hugo
```
sudo dnf install snapd
sudo systemctl enable --now snapd.socket
sudo ln -s /var/lib/snapd/snap /snap
sudo snap install hugo
```


## Quickstart
Go to user home dir
hugo new site quickstart

```
 hugo server --watch --logLevel info --buildDrafts --cleanDestinationDir --disableFastRender --baseURL http://192.168.29.12:1313 --bind 0.0.0.0
```


## Firewall local Hugo server
```
sudo firewall-cmd --add-port=1313/tcp
sudo firewall-cmd --runtime-to-permanent
```

## Git submodules
git submodule add https://github.com/vaga/hugo-theme-m10c.git themes/m10c
git submodule add git@github.com:marcelvenema/hugo-theme-marcelvenema-com.git themes/marcelvenema

