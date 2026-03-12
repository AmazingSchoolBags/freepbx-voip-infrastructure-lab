# Infrastructure VoIP avec FreePBX

Projet réalisé dans le cadre d’un TP d’infrastructure réseau.

L'objectif était de concevoir et sécuriser un standard téléphonique VoIP complet basé sur **Asterisk / FreePBX**.

---

## Architecture

Le système repose sur :

- FreePBX
- Asterisk
- Extensions SIP
- Files d'attente
- IVR
- Conditions temporelles
- Firewall
- Fail2Ban

---

## Fonctionnalités mises en place

### Standard téléphonique (IVR)

Menu vocal permettant de rediriger les appels vers différents services :

- Support technique
- Service commercial
- Comptabilité
- Accueil

---

### Files d'attente

Distribution automatique des appels vers les agents disponibles.

---

### Gestion des horaires

- Horaires d'ouverture
- Message hors horaires
- Pause déjeuner

---

### Mode urgence

Activation d'un flux d'appel spécifique en cas d'urgence.

---

### Call Parking

Possibilité de mettre un appel en attente sur un slot et de le récupérer depuis un autre poste.

---

### Follow-Me

Redirection intelligente des appels vers plusieurs extensions.

---

### Sécurité

#### Firewall UFW

Ports autorisés uniquement pour les réseaux internes :

- SSH
- HTTP (console FreePBX)
- SIP
- RTP

#### Fail2Ban

Protection contre :

- attaques brute force SSH
- attaques SIP

Les adresses IP suspectes sont automatiquement bannies.

---

## Tests réalisés

- appels internes
- navigation IVR
- files d'attente
- conditions horaires
- mode urgence
- call parking
- follow-me
- simulation d’attaque SIP avec bannissement Fail2Ban

---

## Rapport complet

Le rapport détaillé du projet est disponible ici :

TP_Final_FreePBX_Mohamed_Chaouay.pdf
