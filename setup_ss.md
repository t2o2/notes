# Installing and running shadowsocks on Ubuntu Server

## 16.10 yakkety and above

1. Install the the `shadowsocks-libev` package from apt repository.

        sudo apt update
        sudo apt install shadowsocks-libev

1. Save `ss.json` as `/etc/shadowsocks-libev/config.json`.

1. Replace **server_port** and **password** in `ss.json` with your own choices.

1. Restart the `shadowsocks-libev` service.

        sudo systemctl restart shadowsocks-libev
        sudo systemctl status shadowsocks-libev



```
# ss.json
{
    "server": "0.0.0.0",
    "server_port": "[port]",
    "password": "[password]",
    "timeout": 300,
    "method": "xchacha20-ietf-poly1305",
    "mode": "tcp_only",
    "fast_open": true,
    "nameserver": "8.8.8.8"
}
```

