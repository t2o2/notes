# Installing and running shadowsocks on Ubuntu Server

## 16.10 yakkety and above

1. Install the the `shadowsocks-libev` package from apt repository.

        sudo apt update
        sudo apt install shadowsocks-libev

1. Save `ss.json` as `/etc/shadowsocks-libev/config.json`.

        sudo vim /etc/shadowsocks-libev/config.json

1. Replace **server_port** and **password** in `ss.json` with your own choices.

1. Restart the `shadowsocks-libev` service.

        sudo systemctl restart shadowsocks-libev
        sudo systemctl status shadowsocks-libev



```
# ss.json
{
    "server":["::1", "0.0.0.0"],
    "mode":"tcp",
    "server_port":8388,
    "local_port":1080,
    "password":"",
    "timeout":86400,
    "method":"chacha20-ietf-poly1305"
}
```

