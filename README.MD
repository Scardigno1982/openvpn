export CLIENTNAME=Jose

docker-compose run --rm openvpn easyrsa build-client-full $CLIENTNAME nopass

clave del server

docker-compose run --rm openvpn ovpn_getclient $CLIENTNAME > $CLIENTNAME.ovpn