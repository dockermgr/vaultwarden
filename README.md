
# Welcome to vaultwarden installer 👋

## Description

### Requires scripts to be installed

```shell
sudo bash -c "$(curl -LSs <https://github.com/dockermgr/installer/raw/main/install.sh>)"
dockermgr --config && dockermgr install scripts
```

#### Automatic install/update

```shell
dockermgr install vaultwarden
```


#### Manual install

```shell
git clone https://github.com/dockermgr/vaultwarden "$HOME/.local/share/CasjaysDev/dockermgr/vaultwarden"
bash -c "$HOME/.local/share/CasjaysDev/dockermgr/vaultwarden/install.sh"
```

#### Just run it

```shell
git clone <https://github.com/dockermgr/vaultwarden> "$HOME/.local/share/CasjaysDev/dockermgr/vaultwarden"

sudo docker run -d \
--name="vaultwarden" \
--hostname "vaultwarden" \
--restart=always \
--privileged \
-e TZ="${TZ:-${TIMEZONE:-America/New_York}}" \
-p 8082:8082 \
casjay/vaultwarden 1>/dev/null
```

## Author

👤 **Jason Hempstead**

