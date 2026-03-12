# Infrastructure VoIP avec FreePBX

Projet réalisé dans le cadre d’un TP d’administration systèmes et réseaux.

L’objectif du projet était de concevoir, configurer et sécuriser une infrastructure VoIP complète basée sur **Asterisk / FreePBX**.

---

## Technologies utilisées

- FreePBX
- Asterisk
- SIP
- UFW Firewall
- Fail2Ban
- Debian / Linux

---

## Fonctionnalités mises en place

### Standard téléphonique (IVR)

Création d’un menu vocal permettant de rediriger les appels vers différents services.

### Files d’attente (Queues)

Distribution automatique des appels vers les agents disponibles.

### Gestion des horaires

- horaires d’ouverture
- message hors horaires
- pause déjeuner

### Mode urgence

Activation d’un flux d’appel spécifique pour rediriger automatiquement les appels vers une messagerie dédiée.

### Call Parking

Mise en attente d’un appel sur un slot récupérable depuis un autre poste.

### Follow-Me

Redirection intelligente des appels vers plusieurs extensions.

---

## Sécurité

### Firewall UFW

Restriction des accès aux réseaux internes :

- SSH
- HTTP (console FreePBX)
- SIP
- RTP

### Fail2Ban

Protection contre :

- attaques brute force SSH
- attaques SIP

Test de bannissement automatique d’une adresse IP malveillante.

---

## Tests réalisés

- appels internes
- navigation dans l’IVR
- fonctionnement des files d’attente
- gestion des horaires
- activation du mode urgence
- call parking
- follow-me
- test de sécurité Fail2Ban

---

## Rapport détaillé

Le rapport complet du projet est disponible ici :

TP_Final_FreePBX_Mohamed_Chaouay.pdf
