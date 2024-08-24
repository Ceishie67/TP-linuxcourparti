# Sujet réseau

![Alt text](capture%20d'écran/image.png)


# Partie 1 : Setup du patron

### 🌞 Créez une VM avec VirtualBox, nommée Patron

![Alt text](capture%20d'écran/patron.png)

### 🌞 Configurez la VM avec 2 interfaces réseaux. La première en NAT et la deuxième en Host-Only.

La première en NAT :

![Alt text](capture%20d'écran/NAT.png)

La seconde en Host_Only :

![Alt text](capture%20d'écran/Host_Only.png)


### 🌞 Installez Rocky Linux minimal sur la VM.

```
cat /etc/os-release
```
![Alt text](capture%20d'écran/rocky-linux.png)

### 🌞 Définissez une IP statique à la VM.


```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8

```
![Alt text](capture%20d'écran/IP.png)


### 🌞 Donnez un hostname à la machine.

pour lui donner un hostname
```
sudo hostname
```

pour verifier le hostname de la machine
```
hostname
```
![Alt text](capture%20d'écran/Hostname.png)


### 🌞 Configurez SSH pour administrer la machine (avec échange de clés).

 je sais pas faire 

# Partie 2 : Premier test réseau

### 🌞 Configurez correctement ces 2 VM.

### Etudiant
```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/etudiant.png)

```
sudo hostname
hostname
```
![Alt text](capture%20d'écran/hostnameEtudiant.png)

### Mentor

```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/Mentor.png)

```
sudo hostname
hostname
```

![Alt text](capture%20d'écran/hostnameMentor.png)

### 🌞 Testez la connectivité entre les deux machines avec un ping.

#### etudiant vers mentor

![Alt text](capture%20d'écran/ping_Etudiant_vers_Mentor.png)

#### Mentor vers Etudiant

![Alt text](capture%20d'écran/ping_Mentor_vers_Etudiant.png)

# Partie 3 : Un petit peu de routage

### 🌞 Configurez correctement ces 3 VM.

### Mentor

```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/Mentor.png)


### Etudiant
```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```

![Alt text](capture%20d'écran/etudiant2.png)


### Routeur

```
sudo nano /etc/sysconfig/network-scripts/ifcfg-enp0s8
```
![Alt text](capture%20d'écran/Routeur.png)


### 🌞 Testez la connectivité entre les machines :

#### Etudiant vers Routeur :

![Alt text](capture%20d'écran/etudiant_vers_routeur.png)

#### Mentor vers Routeur :

![Alt text](capture%20d'écran/Mentor_vers_routeur.png)

#### Etudiant vers Mentor

![Alt text](capture%20d'écran/ping_étudiant_vers_Mentor.png)