# Red-Team

## **LINUX NETWORK COMMANDS**

|Command | Description |
| --- | --- |
| watch ss -tp | Network connections |
| netstat -ant | Tcp connections -anu=udp |
| netstat -tulpn | Connections with PIDs |
| lsof -i | Established connections |
| smb:// ip /share | Access windows smb share |
| smbclient -0 user\\\\ ip \\ share | SMB connect |
| share user x.x.x.x c$ | Mount Windows share |
| ifconfig eth# ip / cidr | Set IP and netmask |
| ifconfig ethO:1 ip / cidr | Set virtual interface |
| route add default gw gw_ip | Set GW |
| ifconfig eth# mtu [size] | Change MTU size |
| export MAC=xx: XX: XX: XX: XX: XX | Change MAC |
| ifconfig int hw ether MAC | Change MAC |
| macchanger -m MAC int  | Backtrack MAC changer |
| iwlist int scan | Built-in wifi scanner |
| dig -x ip | Domain lookup for IP |
| host ip | Domain lookup for IP |
| dig @ ip domain -t AXrR | DNS Zone Xfer |
| ip xfrm state list | Print existing VPN keys |
| ip addr add ip / cidr dev eth0 | Adds 'hidden' interface |
| /var/log/messages | grep DHCP | List DHCP assignments |
| tcpkill host ip and port port | Block ip:port |
| echo "1" /proc/sys/net/ipv4/ip_forward | Turn on IP Forwarding |
| echo ''nameserver x.x.x.x'' /etc/resolv.conf | Add DNS Server |
