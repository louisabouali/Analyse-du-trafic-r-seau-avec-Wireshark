# Analyse-du-trafic-r-seau-avec-Wireshark

## Objectif
Ce projet permet de capturer et d’analyser des paquets réseau tout en protégeant les données sensibles.

## Étapes du Projet
1. Installation de Wireshark et capture du trafic réseau.
2. Analyse des protocoles (HTTP, DNS, TCP).
3. Anonymisation des adresses IP avec `tcprewrite`.
4. Floutage des informations sensibles dans les captures d’écran.

## Commandes Utilisées
- Anonymisation des adresses IP :
  ```bash
  tcprewrite --infile=traffic-sample.pcap --outfile=traffic-sample-anonymized.pcap \
  --dstipmap=0.0.0.0/0:192.168.0.0/24 \
  --srcipmap=0.0.0.0/0:10.0.0.0/24

# Ça sert à rien de me pirater, j’ai flouté mes adresses IP sensibles ! ;) 