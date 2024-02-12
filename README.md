

# WORK IN PROGRESS!!


## Install hugo
```
sudo dnf install snapd
sudo systemctl enable --now snapd.socket
sudo ln -s /var/lib/snapd/snap /snap
sudo snap install hugo
```


## Quickstart
Go to user home dir
hugo new site quickstart

 hugo server --watch --verbose --buildDrafts --cleanDestinationDir --disableFastRender --baseURL http://192.168.29.12:1313 --bind 0.0.0.0


