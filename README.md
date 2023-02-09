# How-to-made-openvpn-server-on-ubuntu
How-to-made-openvpn-server-on-ubuntu

```
cd ~
mkdir Open_VPN
cd Open_VPN
wget https://raw.githubusercontent.com/angristan/openvpn-install/master/openvpn-install.sh
chmod +x openvpn-install.sh
bash openvpn-install.sh
```

```
Enter
Do you want to enable IPv6 support : n
What port do you want OpenVPN to listen to: 1) Default: 1194
UDP is faster. Unless it is not available, you shouldn't use TCP: 1) UDP
What DNS resolvers do you want to use with the VPN?:  9) Google (Anycast: worldwide)
Do you want to use compression? It is not recommended since the VORACLE attack makes use of it : n
Customize encryption settings? [y/n]: y
Choose which cipher you want to use for the data channel : AES-128-GCM
Choose what kind of certificate you want to use: ECDSA (recommended)
Choose which curve you want to use for the certificate's key: prime256v1 (recommended)
Choose which cipher you want to use for the control channel: ECDHE-ECDSA-AES-128-GCM-SHA256 (recommended)
Choose what kind of Diffie-Hellman key you want to use: ECDH (recommended)
Choose which curve you want to use for the ECDH key: prime256v1 (recommended)
Which digest algorithm do you want to use for HMAC?: SHA-256 (recommended)
tls-auth authenticates the packets, while tls-crypt authenticate and encrypt them: tls-crypt (recommended)
Enter
Enter
```

```
Client name: n-nghia
Do you want to protect the configuration file with a password: Add a passwordless client
```

After that: it will auto gen a profile openvpn on the /root, download it and start to use in client side !
