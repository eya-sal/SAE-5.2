# SAE-5.2
# Projet de Configuration Réseau

Ce projet met en place une infrastructure réseau comprenant plusieurs routeurs, pare-feu, VLANs et configurations DHCP. L'objectif est de fournir un réseau sécurisé et bien structuré avec des machines réparties dans différents VLANs obtenant leurs adresses IP dynamiquement via DHCP.

---

## 🛠️ **Architecture**

### Topologie
- **Routeur externe** : Gère les communications avec l'extérieur.
- **Routeur pare-feu (FW)** : Sécurise les accès réseau.
- **Routeur DHCP** : Fournit des adresses IP dynamiques aux machines des VLANs.
- **Switchs et VLANs** :
  - **Switch S1** : Contient le **VLAN 10** (machines attribuées via DHCP).
  - **Switch S2** : Contient le **VLAN 20** (machines attribuées via DHCP).
  - **Switch S3** : Contient le **VLAN 30** (machines attribuées via DHCP).

---

## 📂 **Étapes du Projet**

Le projet est divisé en plusieurs étapes, chacune correspondant à un commit pour une meilleure traçabilité. Voici les étapes :

### 1️⃣ **Mise en place initiale** (Premier commit)
- Création de la structure réseau de base.
- Ajout des équipements : routeurs, switches et interfaces.

### 2️⃣ **Configuration du routeur externe** (Deuxième commit)
- Configuration de l'interface connectée à l'extérieur.
- Liaison avec l'interface du routeur pare-feu (FW).

### 3️⃣ **Configuration du pare-feu et du DHCP** (Troisième commit)
- Configuration de l'autre interface du pare-feu connectée au réseau interne.
- Mise en place du serveur DHCP sur le routeur interne pour fournir des adresses IP dynamiques.

### 4️⃣ **Création des VLANs et DHCP pour S1** (Quatrième commit)
- Création et configuration du **VLAN 10** sur le **Switch S1**.
- Attribution des adresses IP aux machines du VLAN 10 via DHCP.

### 5️⃣ **Attribution des IPs pour S2** (Cinquième commit)
- Création et configuration du **VLAN 20** sur le **Switch S2**.
- Attribution des adresses IP aux machines du VLAN 20 via DHCP.

### 6️⃣ **Attribution des IPs pour S3** (Dernier commit)
- Création et configuration du **VLAN 30** sur le **Switch S3**.
- Attribution des adresses IP aux machines du VLAN 30 via DHCP.

---

## 🧰 **Outils et Technologies Utilisés**
- **Routeurs et switches simulés** : Cisco Packet Tracer.
- **DHCP** : Configuration pour fournir des IP dynamiques.
- **Pare-feu** : Sécurisation des accès réseau.
- **VLANs** : Isolation et segmentation du réseau.


