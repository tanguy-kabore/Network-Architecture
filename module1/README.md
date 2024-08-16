# Guide du TD1 - VLSM et Routage Statique
[Cliquez ici au besoin pour retourner sur la page principale](../README.md).

## Objectifs du TD1

L'objectif de ce TD est de s'exercer à l'utilisation du VLSM (Variable Length Subnet Mask). Les objectifs spécifiques sont :
> **Note :** Télécharger les canevas des differents tabeaux avant de continuer: [network_informations.xlsx](../assets/module1/network_informations.xlsx).

1. **Réalisation d'un Tableau d'Adressage de Sous-Réseau :**
   - Créez un tableau d'adressage pour les sous-réseaux et remplissez la feuille **`networks`** du fichier Excel.

2. **Tableau d'Adressage des Interfaces :**
   - Établissez un tableau d'adressage pour les interfaces et complétez la feuille **`interfaces`** du fichier Excel.

3. **Table de Routes Statiques :**
   - Introduisez le routage statique en créant une table de routes statiques et remplissez la feuille **`static routes`** du fichier Excel.

4. **Mini TP :**
   - Réalisez un mini TP portant sur l'introduction aux configurations des interfaces et aux routes statiques.

## Guide du TP Appliqué au TD1

### Prérequis

Avant de commencer le TP, assurez-vous de disposer du logiciel **Cisco Packet Tracer**. Ce logiciel est essentiel pour simuler et configurer des réseaux virtuels. Il vous permet de :

- **Concevoir des Réseaux :** Créez des modèles de réseaux et visualisez-les.
- **Développer des Compétences :** Résolvez des problèmes algorithmiques liés aux réseaux.
- **Difficultés de Conception :** Travaillez sur des problèmes avec plusieurs solutions correctes.
- **Résolution de Problèmes :** Diagnostiquez et corrigez des réseaux simulés.

#### Téléchargement et Installation de Cisco Packet Tracer

Pour obtenir et installer Cisco Packet Tracer, suivez ces étapes :

1. **Téléchargez la version appropriée :**
   - **[MacOS 64bit](https://sgp-ui-components.s3.amazonaws.com/s/ff9e491c-49be-4734-803e-a79e6e83dab1/resources/de225808-e31a-42ec-9528-7ac8dc95aebf/v1/en-US/Packet_Tracer822_setup_mac_signed.dmg?response-cache-control=no-cache&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240816T154758Z&X-Amz-SignedHeaders=host&X-Amz-Expires=30&X-Amz-Credential=AKIAUJZRIEYBKYV2WA5Q%2F20240816%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=2d42b18ad7ca87150cd6772875dbf0fc6efd11c8453829844a6c91d3d5d5c22c)**
   - **[Ubuntu 64bit](https://sgp-ui-components.s3.amazonaws.com/s/ff9e491c-49be-4734-803e-a79e6e83dab1/resources/9accb7fd-7560-45c6-b6de-9ab7e9cf07b8/v1/en-US/Packet_Tracer822_amd64_signed.deb?response-cache-control=no-cache&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240816T154735Z&X-Amz-SignedHeaders=host&X-Amz-Expires=30&X-Amz-Credential=AKIAUJZRIEYBKYV2WA5Q%2F20240816%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=b081b5b23a871cbbf12099796de34ce4bf49a29fada9220ce016bb49a297b1b2)**
   - **[Windows 64bit](https://sgp-ui-components.s3.amazonaws.com/s/ff9e491c-49be-4734-803e-a79e6e83dab1/resources/8f1527f7-f188-4655-909a-8199135ac6d8/v1/en-US/Packet_Tracer822_64bit_setup_signed.exe?response-cache-control=no-cache&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240816T154510Z&X-Amz-SignedHeaders=host&X-Amz-Expires=30&X-Amz-Credential=AKIAUJZRIEYBKYV2WA5Q%2F20240816%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=750ba2bf3de5eb781318d715d710e6f20ae4cdf49f1cc5a4e4f44068d117dcff)**

2. **Lancez le programme d'installation de Packet Tracer.**
3. **Démarrez Cisco Packet Tracer en sélectionnant l'icône appropriée.**
4. **Cliquez sur le bouton vert "Skills For All" pour vous authentifier.**
5. **Packet Tracer se lancera et vous pourrez explorer ses fonctionnalités.**

Pour des instructions détaillées, référez-vous au document [Instructions de Téléchargement et d'Installation de Cisco Packet Tracer](../assets/module1/Cisco_Packet_Tracer_Download_and_Installation_Instructions.pdf).

#### Configuration Requise

- **Système d'exploitation :** Windows 10/11, MacOS 10.14 ou plus récent, Ubuntu 20.04/22.04 LTS
- **Processeur :** AMD64 (x86-64)
- **RAM :** 4 Go
- **Espace disque libre :** 1,4 Go

## Étapes du TP

> **Note :** Consultez le document [Guide to Cisco Routers Configuration Becoming a Router Geek.pdf](../assets/module1/Guide_to_Cisco_Routers_Configuration_Becoming_a_Router_Geek.pdf) pour des ressources supplémentaires.

### Étape 1 : Création de la Topologie Réseau

1. **Sélectionnez la série de routeurs CISCO 1841** dans Packet Tracer.
2. **Ajoutez le module HWIC2T** pour obtenir les ports série. N'oubliez pas d'éteindre le routeur avant d'ajouter les modules, puis rallumez-le après.
3. **Utilisez des câbles série** pour interconnecter les routeurs.
4. **Pour les switches, choisissez la série Cisco 2960.**

### Étape 2 : Configuration des Interfaces

- Configurez les interfaces des routeurs en vous servant du tableau d'adressage des interfaces du fichier Excel.
- Connectez au moins un PC à chaque switch et configurez l'interface du PC avec une adresse IP utilisable.

### Étape 3 : Configuration des Routes Statiques

- Configurez les routes statiques des routeurs en utilisant le tableau des routes du fichier Excel.

### Étape 4 : Testez la Connectivité de Votre Réseau

- Utilisez la commande `ping` du protocole ICMP pour vérifier la connectivité entre les dispositifs de votre réseau.

## Contact

Pour toute question ou commentaire, n'hésitez pas à me contacter :
- **Par e-mail :** [tanguykabore@yahoo.fr](mailto:tanguykabore@yahoo.fr)
- **Par WhatsApp :** +226 75643226

Bon apprentissage et bonne configuration !