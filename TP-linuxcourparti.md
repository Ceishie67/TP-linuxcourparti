# Sujet réseau

![Alt text](capture%20d'écran/image.png)


# Partie 1 : Setup du patron

🌞 Créez une VM avec VirtualBox, nommée Patron

![Alt text](capture%20d'écran/patron.png)

🌞 Configurez la VM avec 2 interfaces réseaux. La première en NAT et la deuxième en Host-Only.

La première en NAT :

![Alt text](capture%20d'écran/NAT.png)

La seconde en Host_Only :

![Alt text](capture%20d'écran/Host_Only.png)


🌞 Installez Rocky Linux minimal sur la VM.

```
cat /etc/os-release
```
![Alt text](capture%20d'écran/rocky-linux.png)

🌞 Définissez une IP statique à la VM.


```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8

```
![Alt text](capture%20d'écran/IP.png)


🌞 Donnez un hostname à la machine.

pour lui donner un hostname
```
sudo hostname
```

pour verifier le hostname de la machine
```
hostname
```
![Alt text](capture%20d'écran/Hostname.png)


🌞 Configurez SSH pour administrer la machine (avec échange de clés).

 je sais pas faire 

# Partie 2 : Premier test réseau

🌞 Configurez correctement ces 2 VM.

## Etudiant
```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/etudiant.png)

```
sudo hostname
hostname
```
![Alt text](capture%20d'écran/hostnameEtudiant.png)

## Mentor

```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/Mentor.png)

```
sudo hostname
hostname
```

![Alt text](capture%20d'écran/hostnameMentor.png)
