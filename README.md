# L'anonymat en ligne #

# 1 - Le Client Tor #

## 1.1 - Information  #
Tor fonctione en décentralisant tout son réseau, lorsque vous faites une recherche votre connexion passe par celle d'autres personnes acceptant de faire partie du réseau.C'est cette structure décentralisé qui permet au réseau d'être quasi intouchable.
Lorsqu'on utilise wireshark avec tor on remarque que notre ip de destination et du client change constamment.
Deplus les données sont chiffrés.

## 1.2 - Avantage # 

Tor comme vu plus haut permet permet un anonymat presque total, et reste plus simple d'installation.

## 1.3 - Inconvénient #

Les inconvénients de Tor existe pourtant le premier c'est qu'il est conseiller d'utiliser un vpn ou l'hidden service de tor protége les données sur le dernier noeud de sortie, et le second est que le client est trés lent, comme la connexion passe par divers relais.

# 2 - Hidden Service Tor #

## 2.1 - Information  #
On remarquera qu'avec l'Hidden service, le dernier noeud de notre chaine est le site onion, cela permet une certaine protection en bout de chaine.On remarque qu'avec Wireshark que la dernier ip du noeud est celle de la vm.

## 2.2 - Avantage #

L'installation est plutôt facile, et cela permet un annonymat complet, l'hidden service agit presque comme un VPN.

## 2.3 - Inconvéniant #
Les recherches sont toujours trés longue, et cela n'accélére pas celle-ci.

## 2.4 Screens

<img src="https://github.com/Fipk/Reseau_TP4/blob/master/images/hidden.png"></img>

# 3 - Le Proxy # 

## 3.1 - Information  #

Lorsqu'on utilise Wireshark pour écouter, on remarque que les requêtes sont toutes renvoyer vers l'IP du proxy et non pas celle du site demander.

## 3.2 - Avantage #
Le proxy permet d'interdire les ordinateurs d'internet de venir se connecter au votre, en fonction du proxy que vous utiliser certains peuvent vous permettre de masquer certaines informations complémentaire ( Os, moteur de recherche). La géolocalisation est aussi compliqué.
## 3.3 - Inconvénient #
Le soucis du proxy est qu'il utilise un service externe que vous ne pouvez gérez, toutes mes informations passe maintenant par numéricable et ceci pourais trés bien récupéré mes données de connexion.

## 3.4 Screens

<p> Proxy http</p>
<img src="https://github.com/Fipk/Reseau_TP4/blob/master/images/proxy_http.PNG"></img>

<p> Proxy https</p>
<img src="https://github.com/Fipk/Reseau_TP4/blob/master/images/proxy_https.PNG"></img>

# 4 - Doh / Dot :

## 4.1 - Information  #

Avec Wireshark on peut voir que mes données sont chiffrés, et que cela rend imposible la lecture des informations.

## 4.2 - Avantage #
L'avantage du Doh c'est que cette technologie permet un véritable chiffrement des données et évite leurs modifications par une personne autre que l'utilisateur.

## 4.3 - Inconvénient  #
L'inconvénient de Doh, dot est qu'il utilise à outrance HTTPS, il faut tout passer par cela, certains sites peuvent bloquer l'accés.