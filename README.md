# docker-compose
这是一个个人实验性质的游戏工具实现，采用 openvpn + udp2raw + UDPspeeder
关于openvpn的配置参考 https://github.com/kylemanna/docker-openvpn/blob/master/docs/docker-compose.md

openvpn需要修改服务器配置文件 添加以下两行
```
mssfix 1240
tun-mtu 1240
```
生成的ovpn配置文件自己手动加上上面两行
然后端口和ip改成自己udp2raw配置的。
