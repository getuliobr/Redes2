# Roteamento Estatico
## GNS3
```sh
# Configurar IP por placa de rede
ifconfig <placaDeRede> <ip> netmask <mascara>
# Adicionar rotas
route add default gw <ip>
# Configurar DNS
echo <servidorDNS> >> /etc/resolv.conf
```

## CISCO
```sh
enable
configure terminal

# Configurar IP por interface
interface <nomeInterface>
ip address <ip> <mask>
no shutdown

# Adicionar rotas
ip route <ipDestino> <mascaraIpDestino> <ipRoteadorAcessoDestino>
```
