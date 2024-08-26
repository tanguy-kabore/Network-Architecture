# Étude de Cas : Conception et Configuration d'un Réseau d'Entreprise

## Contexte

Dans le cadre de ce projet, vous êtes engagés pour concevoir et configurer un réseau pour une entreprise fictive. L'entreprise dispose de plusieurs départements répartis sur différents étages d'un bâtiment. Chaque département doit être isolé des autres par des VLANs, et une connectivité sécurisée doit être mise en place entre les différents segments du réseau.

## Objectifs

Ce projet vise à vous familiariser avec la conception et la mise en œuvre d'un réseau d'entreprise complet. Vous serez évalués sur la conception, la configuration, et la documentation de votre réseau. Assurez-vous de suivre les bonnes pratiques de sécurité et d'efficacité réseau tout au long du projet. De facon spécifique, il s'agira de:

- Concevoir l'architecture réseau de l'entreprise en utilisant une adresse réseau donnée.
- Créer plusieurs sous-réseaux pour les différents départements.
- Configurer les adresses IP des interfaces sur les routeurs et les switches.
- Configurer le routage entre les différents sous-réseaux.
- Mettre en place un serveur DHCP pour la distribution des adresses IP.
- Configurer un serveur DNS pour la résolution de noms.
- Installer et configurer un serveur Web accessible depuis tous les sous-réseaux.
- Appliquer les principes de commutation avancée, notamment le VTP et le Spanning Tree Protocol (STP).
- Mettre en place et configurer des VLANs pour chaque département.
- Configurer les accès distants sécurisés sur les routeurs et les switches (SSH).
- Créer des ACL standard et étendues pour restreindre l'accès entre les VLANs selon les besoins.

## Étapes à Suivre

### 1. **Conception du Réseau**

   - **Adresse Réseau** : L'adresse réseau de base à utiliser est `192.168.0.0/16`.
   - **Sous-réseaux** : Divisez l'adresse réseau en plusieurs sous-réseaux pour les départements suivants :
     - Administration
     - Ressources Humaines
     - IT
     - Finance
     - Marketing
   - **VLANs** : Créez un VLAN distinct pour chaque département.

### 2. **Configuration des Interfaces**

   - Assignez les adresses IP aux interfaces des routeurs et des switches selon la topologie définie.
   - Configurez les interfaces pour le routage inter-VLAN sur le routeur.
   - Assurez-vous que les interfaces de trunking entre les switches et les routeurs sont correctement configurées.

### 3. **Configuration du Routage**

   - Configurez le routage statique ou dynamique pour assurer la communication entre les différents sous-réseaux.
   - Vérifiez que le routage fonctionne correctement à l'aide de tests de connectivité (ping).

### 4. **Serveur DHCP**

   - Configurez un serveur DHCP pour fournir dynamiquement des adresses IP aux postes clients dans chaque VLAN.
   - Assurez-vous que les clients reçoivent les adresses IP correctes et les informations de passerelle par défaut.

### 5. **Serveur DNS**

   - Configurez un serveur DNS pour gérer la résolution de noms dans le réseau.
   - Assurez-vous que tous les clients peuvent résoudre les noms de domaine correctement.

### 6. **Serveur Web**

   - Installez et configurez un serveur Web accessible depuis tous les sous-réseaux.
   - Assurez-vous que le serveur est accessible via son nom de domaine résolu par le DNS.

### 7. **Commutation Avancée**

   - Configurez le VTP pour gérer les VLANs de manière centralisée sur les switches.
   - Configurez le Spanning Tree Protocol (STP) pour éviter les boucles dans le réseau.
   - Changez le VLAN natif si nécessaire pour renforcer la sécurité.

### 8. **Accès Distant Sécurisé**

   - Activez et configurez SSH pour l'accès distant sécurisé aux switches et routeurs.
   - Désactivez l'accès Telnet pour améliorer la sécurité.

### 9. **Configuration des ACL**

   - Créez des listes de contrôle d'accès (ACL) standard pour restreindre l'accès à certains sous-réseaux.
   - Créez des ACL étendues pour filtrer le trafic en fonction de critères plus spécifiques, comme l'adresse source, la destination, ou le type de protocole.

### 10. **Validation du Réseau**

   - Testez toutes les configurations en vérifiant que les clients dans chaque VLAN peuvent accéder aux ressources nécessaires (Web, DNS, etc.).
   - Vérifiez l'efficacité des ACL en testant les accès bloqués ou autorisés entre les VLANs.

## Livrables

1. **Diagramme Réseau** : Un schéma complet de votre réseau, avec les adresses IP assignées et les VLANs configurés.
2. **Configurations** : Les configurations complètes des switches, routeurs, et serveurs (DHCP, DNS, Web).
3. **Rapport de Validation** : Un rapport décrivant les tests effectués pour valider la configuration et les résultats obtenus.