# Sujet réseau

![Alt text](image.png)


# Partie 1 : Setup du patron

🌞 Créez une VM avec VirtualBox, nommée Patron

![Alt text](patron.png)

🌞 Configurez la VM avec 2 interfaces réseaux. La première en NAT et la deuxième en Host-Only.

La première en NAT :

![Alt text](NAT.png)

La seconde en Host_Only :

![Alt text](Host_Only.png)


🌞 Installez Rocky Linux minimal sur la VM.

```
cat /etc/os-release
```
![Alt text](rocky-linux.png)

🌞 Définissez une IP statique à la VM.


```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8

```
![Alt text](IP.png)


🌞 Donnez un hostname à la machine.

pour lui donner un hostname
```
sudo hostname
```

pour verifier le hostname de la machine
```
hostname
```
![Alt text](Hostname.png)
