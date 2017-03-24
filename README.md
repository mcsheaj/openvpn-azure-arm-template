## Open VPN Azure ARM Template ##

ARM template to setup open vpn server in Microsoft Azure.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https://raw.githubusercontent.com/smattoo/openvpn-azure-arm-template/master/openvpn-azuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=Frahttps://raw.githubusercontent.com/smattoo/openvpn-azure-arm-template/master/openvpn-azuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

### Steps ###

- Update the template parameters as required.
- Run the template
- Copy the **client1.ovpn**(~/client-configs/files/) from the provisioned ubuntu virtual machine `scp <username>@dgopenvpnserver.<location>.cloudapp.azure.com:/client-configs/files/client1.ovpn /some/local/directory`
- Install the openvpn client from here([64-bit](https://swupdate.openvpn.org/community/releases/openvpn-install-2.3.14-I602-x86_64.exe "OpenVpnClient-64-Bit"), [32-bit](https://swupdate.openvpn.org/community/releases/openvpn-install-2.3.14-I602-i686.exe "OpenVpnClient-32-Bit"))
- Post above install copy the **client1.ovpn** file under C:\Program Files\OpenVPN\config and connect to the server.
- Hurray! Open VPN connection should be established.
