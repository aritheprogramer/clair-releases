# Clair — bêta gratuite

Clair est une application indépendante pour consulter son compte ÉcoleDirecte, ses notes, son agenda et ses messages, avec un assistant IA. Ce n’est pas une application officielle d’ÉcoleDirecte.

## Android : installation sans compte Expo

1. Depuis ton téléphone Android, [télécharge Clair](https://github.com/aritheprogramer/clair-releases/releases/download/android-beta-2/Clair-Android.apk) (environ 128 Mo).
2. Ouvre le fichier `Clair-Android.apk`. Si Android le demande, autorise ton navigateur à installer cette application, puis confirme l’installation. Tu peux retirer cette autorisation ensuite.
3. Ouvre **Clair**, puis connecte-toi avec **ton propre compte ÉcoleDirecte**. Réponds toi-même au QCM ou au code de vérification éventuel.
4. Active **Rester connecté sur cet appareil** si tu souhaites la reconnexion automatique.

Pas besoin d’Expo Go, de compte Expo, de compte GitHub ou du Wi-Fi du créateur. Il s’agit d’une bêta à installer directement, pas d’une publication Google Play. Les prochaines versions APK pourront être installées par-dessus celle-ci.

## iPhone : IPA à signer soi-même

Un [IPA non signé](https://github.com/aritheprogramer/clair-releases/releases/download/ios-unsigned-beta-1/Clair-unsigned.ipa) est disponible pour un test personnel sans compte Expo. Il faut le signer avant installation, par exemple avec AltStore Classic et son propre compte Apple gratuit ; la signature expire après 7 jours. [Lire le guide IPA](INSTALL_IPA.md). Ce n’est pas une installation directe depuis Safari, ni une publication App Store. Installation sur appareil après signature non vérifiée.

## iPhone : bêta sur invitation dans Expo Go

1. Installe [Expo Go](https://expo.dev/go) et crée ton [compte Expo gratuit](https://expo.dev/signup).
2. Transmets **uniquement l’adresse e-mail de ton compte Expo** à l’organisateur du test, en privé, pour recevoir une invitation Viewer à l’équipe **squidapps22’s team**.
3. Accepte l’invitation, puis connecte-toi avec ce même compte dans Expo Go.
4. Affiche [le QR code de Clair](https://qr.expo.dev/eas-update?projectId=2cc20485-5d1a-4eea-aee4-e1956d28e756&groupId=57fe8880-0362-492a-bb39-d9390db69da9) sur un autre écran et scanne-le avec l’appareil photo de ton iPhone. [Prévisualisation Expo Go](https://expo.dev/preview/update/expo-go?projectId=2cc20485-5d1a-4eea-aee4-e1956d28e756&group=57fe8880-0362-492a-bb39-d9390db69da9).
5. Dans Clair, connecte-toi à ton propre compte ÉcoleDirecte. Active **Rester connecté sur cet appareil** si tu le souhaites.

L’iPhone reste une bêta sur invitation : ce lien n’est pas une installation publique via l’App Store ou TestFlight. Chacun utilise son propre compte Expo, jamais celui du créateur. Si Clair disparaît des projets récents après « Clear » ou si la liste affiche « No projects yet », rescanner le QR code.

## Agenda adapté aux annonces scolaires

Les plannings d’examens peuvent désormais ajouter des épreuves dans l’agenda pour la classe et les matières de l’élève. Les cours entièrement couverts sont marqués remplacés ; les chevauchements partiels restent à vérifier. Chaque détection renvoie au message source et peut être ignorée. Les PDF/TXT lisibles sont analysés, avec une indication lorsqu’une pièce jointe ne peut pas être lue. Les sources accessibles sont celles d’ÉcoleDirecte : aucune boîte mail personnelle n’est connectée.

## Ce qui change dans cette version

- Affichage des données déjà enregistrées dès l’ouverture, puis actualisation en arrière-plan de l’interface.
- Reconnexion ÉcoleDirecte avec les identifiants enregistrés localement, lorsqu’une nouvelle vérification n’est pas exigée.
- Résumé centré sur les cours d’aujourd’hui et le travail pour demain ; le trimestre reste disponible dans le contexte de l’assistant.
- Accès direct à la conversation depuis l’accueil ; réponses avec titres, listes et tableaux lisibles.
- Accent vivant sur 20 nuances, nouvelle présentation de la connexion et du QCM, davantage de retours haptiques.

## Données et limites du test

Les identifiants mémorisés sont conservés dans le stockage sécurisé du téléphone. Ils transitent par HTTPS vers le serveur Clair pour la connexion à ÉcoleDirecte ; Clair ne les conserve pas dans sa base serveur. Les données scolaires synchronisées et les sessions sont traitées par le serveur hébergé. Les fonctions IA transmettent le contexte scolaire utile à Groq. Ne communique jamais ton mot de passe ou tes codes à l’organisateur. Tu peux effacer les identifiants locaux depuis ton profil.

Le serveur gratuit peut prendre environ une minute à se réveiller après une période d’inactivité. Une première connexion nécessite Internet ; les données déjà enregistrées peuvent s’afficher hors ligne. L’actualisation toutes les 30 minutes fonctionne lorsque l’application est au premier plan, avec rattrapage à la reprise : ce n’est pas une tâche garantie lorsque le téléphone ferme l’application. ÉcoleDirecte peut toujours demander une nouvelle vérification de sécurité. Ne compte pas sur cette bêta pour une notification urgente.

Cette version a passé ses tests automatisés et ses compilations iOS/Android ; son rendu et ses interactions sur les téléphones des testeurs restent à vérifier. Pour signaler un problème, indique le modèle du téléphone, les étapes et le message d’erreur. Masque les données personnelles dans toute capture et n’ajoute aucune donnée scolaire privée dans une issue publique.

## Version

Bêta Android 2 — version 1.0.0, build 2, publiée le 6 octobre 2026. iPhone : publication du 6 octobre 2026, groupe `57fe8880-0362-492a-bb39-d9390db69da9`.

SHA-256 de l’APK : `807b9a4cc9081bf260e6f8efa08008ffd28b663c53720691d826c3d12d2a97af`.
