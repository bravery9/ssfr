 ssfr - A port forward and socks5 tool.
 =

This is ssf tool command simplified version.

Other options can use https://github.com/securesocketfunneling/ssf

Features include：

>(1)socks5 into the lan;
>(2)Port forward.

## Usage
```
usg: ssfr.exe -ssfd "ssfd binding port" [Options]
     ssfr.exe -s5 "remote ssfd binding address" "remote ssfd binding port" "socks5 port"
     ssfr.exe -pf "remote ssfd binding address" "remote ssfd binding port" "Forward port" "local port"

eg1: Use socks5 into the lan.
     (1).Enable ssfd service.(Execute command on the target).
     ssfr.exe -ssfd 49150
     (2).Enable socks5 on the target to forward your local 127.0.0.1:1080.
     ssfr.exe -s5 8.8.8.8 49150 1080
![socks5into](https://raw.githubusercontent.com/FlyfishSec/ssfr/master/Usage/socks5into.png "socks5into.gif")
eg2: Forward the target 3389 port to your local 127.0.0.1:8888.
     (1).Enable ssfd service in your IP(Execute in your Public net IP or base on NAT IP).
     ssfr.exe -ssfd 49150
     (2).Forward the target port 3389 to your local 127.0.0.1:8888.(Execute command on the target)
     ssfr.exe -pf 8.8.8.8 49150 3389 8888
![rdpforward](https://raw.githubusercontent.com/FlyfishSec/ssfr/master/Usage/rdpforward.png "rdpforward.png")
```

	 