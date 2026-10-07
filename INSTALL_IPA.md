# Clair — IPA iPhone non signé

[Télécharger Clair-unsigned.ipa](https://github.com/aritheprogramer/clair-releases/releases/download/ios-unsigned-beta-1/Clair-unsigned.ipa) · environ 19 Mo · iOS 16.4 minimum déclaré.

Ce fichier contient l’application native et son code embarqué. **Il n’est pas signé par Apple : il ne s’installe pas directement depuis Safari ni dans Expo Go.** Il est destiné à une signature personnelle. Sa compilation a réussi ; son installation et son lancement après signature restent à vérifier sur iPhone.

## Installation gratuite avec AltStore Classic

1. Sur ton ordinateur, suis le guide officiel pour installer AltServer et AltStore Classic : [Mac](https://faq.altstore.io/altstore-classic/how-to-install-altstore-macos) ou [Windows](https://faq.altstore.io/altstore-classic/how-to-install-altstore-windows). Le premier passage nécessite ton iPhone connecté à l’ordinateur.
2. Utilise ton propre compte Apple dans l’outil de signature. N’envoie aucun mot de passe ou code dans une conversation ou à l’organisateur.
3. Enregistre l’IPA dans Fichiers sur ton iPhone, puis importe-le dans AltStore Classic depuis **My Apps → +**. Garde AltServer accessible pendant la signature et l’installation.
4. Termine les éventuelles étapes de confiance et de mode développeur décrites dans le guide officiel, puis ouvre Clair et connecte-toi à ton propre compte ÉcoleDirecte.

Avec un compte Apple gratuit, **la signature expire après 7 jours** : utilise **Refresh All** dans AltStore pour la renouveler avec AltServer. Apple limite également le nombre d’applications installées de cette manière. [Fonctionnement et limites officiels](https://faq.altstore.io/altstore-classic/your-altstore).

Il faut **AltStore Classic**, qui permet l’import d’IPA. AltStore PAL n’est pas le même parcours. Aucun abonnement Apple Developer n’a été acheté. Cette méthode est moins simple pour une classe que la bêta Expo Go ; elle n’est ni une publication App Store ni une distribution TestFlight.

## Autre accès : Expo Go

Pour les testeurs déjà invités, [le QR Expo Go](https://qr.expo.dev/eas-update?projectId=2cc20485-5d1a-4eea-aee4-e1956d28e756&groupId=57fe8880-0362-492a-bb39-d9390db69da9) reste disponible, avec leur propre compte Expo. L’IPA fonctionne comme une application distincte d’Expo Go : une première connexion à ÉcoleDirecte y sera nécessaire.

## Cette version

Connexion avec mémorisation sécurisée sur l’appareil, assistant enrichi, personnalisation et agenda adapté aux plannings d’examens identifiés dans les messages. Les épreuves sont sourcées, les cours entièrement couverts sont marqués remplacés et les chevauchements partiels restent à vérifier. Les détections peuvent être ignorées depuis le message source. Les documents PDF/TXT lisibles sont pris en compte ; une pièce jointe inaccessible ou une image scannée peut nécessiter une lecture manuelle.

L’hébergement gratuit peut encore prendre un moment à se réveiller. La reconnexion automatique n’empêche pas ÉcoleDirecte d’exiger une nouvelle vérification. Les données scolaires sont traitées sur le serveur Clair et les fonctions IA utilisent Groq. [Guide général et données](README.md).

Version 1.0.0, build 1, architecture arm64, bundle `app.clair.mobile`. SHA-256 : `621cda786afebe3524deaa2432253cb74f7d09f2dd0a9469923f83d98c0bc816`.
