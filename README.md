# openvpn-xor
Openvpn with Tunnelblick's xor patch applied

Ubuntu 22.04 / Debian 11 (tested on Ubuntu 24.04, openvpn 2.6)

1. Install OpenVPN via Angristan's script (latest)
```
curl -O https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh
```
or from here (Angristan's script)
```
curl -O https://raw.githubusercontent.com/dexxx-x/openvpn-xor-installscript/main/openvpn-install.sh
chmod +x openvpn-install.sh
./openvpn-install.sh
```
2. Remove openvpn package
```
apt remove openvpn -y
```

3. Download and run OpenVPN with xor patch applied script
```
wget https://raw.githubusercontent.com/x0r2d2/openvpn-xor/main/openvpn_xor_install.sh -O openvpn_xor_install.sh 
chmod +x openvpn_xor_install.sh
bash openvpn_xor_install.sh
```

or from here (x0r2d2 script)
```
curl -O https://raw.githubusercontent.com/dexxx-x/openvpn-xor-installscript/main/openvpn-install.sh
chmod +x openvpn_xor_install.sh
bash openvpn_xor_install.sh
```

4. Add/remove clients via Angristan's script (openvpn-install.sh)
```
bash openvpn-install.sh
```

Clients: 

1. Windows: https://github.com/lawtancool/openvpn-windows-xor
2. Android: [VPN Client Pro](https://play.google.com/store/apps/details?id=it.colucciweb.vpnclientpro&hl=en_US&gl=US)
3. iOS: [Passepartout, VPN Client](https://apps.apple.com/us/app/passepartout-vpn-client/id1433648537)
4. Install via script and add config as client to /etc/openvpn/client and create service file or start manually.
5. If you need Openwrt with openvpn xor patch, you can use builder from [HERE](https://github.com/dexxx-x/Xiaomi-router-MI4C/tree/openvpnXOR), just change .config for your router.
