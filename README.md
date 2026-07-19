# 🔥 Comprendre et configurer un firewall — Résumé de formation & mise en pratique

Ce dépôt rassemble mes notes personnelles suite à une formation LinkedIn Learning sur les firewalls, ainsi que les preuves de mise en pratique réalisées sur un lab virtualisé (OPNsense + FortiGate + Windows).

## 📄 Contenu du dépôt

| Fichier | Description |
|---|---|
| [`Firewall_Resume_Formation.pdf`](./Firewall_Resume_Formation.pdf) | Version PDF — lisible directement dans l'aperçu GitHub |
| [`Firewall_Resume_Formation.docx`](./Firewall_Resume_Formation.docx) | Version Word éditable |

## 🖧 Topologie du lab

Un firewall **OPNsense** virtualisé fait l'interface entre un WAN (VMNET8, DHCP) et deux réseaux LAN isolés :

| Réseau | Plage | Passerelle | Machine |
|---|---|---|---|
| LAN (VMNET6) | `10.33.0.0/24` | `10.33.0.254` | Windows 11 |
| LAN 2 (VMNET7) | `192.168.33.0/24` | `192.168.33.254` | Windows 10 |

## 📚 Structure de la formation

| # | Partie | Statut |
|---|---|---|
| 1 | Comprendre le rôle et les fonctions d'un firewall | 📘 Notion théorique |
| 2 | Déployer un firewall réseau et mettre en place les règles principales | ✅ Appliqué |
| 3 | Protéger le réseau des menaces extérieures (redirection de port, VPN nomade WireGuard) | 🔜 À pratiquer |
| 4 | Tester l'efficacité des fonctions configurées et dépanner un firewall | ✅ Partiellement appliqué |
| 5 | Configurer les fonctions réseau avancées (portail captif, VPN site à site IPsec) | 🔜 À pratiquer |
| 6 | Profiter de l'intelligence embarquée sur son firewall (filtrage web, contrôle applicatif, IPS) | ✅ Appliqué |
| 7 | Protéger un poste de travail ou un serveur avec un firewall logiciel | ✅ Appliqué |

Le détail complet (points clés + captures d'écran de chaque manipulation) est disponible dans le [PDF](./Firewall_Resume_Formation.pdf).

## 🛠️ Outils utilisés

- **OPNsense** (pare-feu réseau, virtualisé)
- **FortiGate** (pare-feu réseau, virtualisé)
- **Windows Defender Firewall** (pare-feu logiciel)
- VMware (VMNET6, VMNET7, VMNET8)

## 🎯 Prochaines étapes

- [ ] VPN nomade (WireGuard)
- [ ] VPN site à site (IPsec)
- [ ] Portail captif
- [ ] Scans de test (Nmap/Zenmap, Netcat)

## 📬 Contact

N'hésitez pas à ouvrir une *issue* ou à me contacter sur LinkedIn si vous avez des retours, notamment sur les certifications réseau/cybersécurité (Fortinet NSE, CCNA Security, CompTIA Security+...) — je suis en pleine réflexion sur la suite de mon parcours.
