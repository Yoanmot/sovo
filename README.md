# Sovo

Dictée vocale gratuite qui tourne entièrement sur ton ordinateur. Tu maintiens une touche, tu parles, tu relâches : le texte s'écrit là où se trouve ton curseur, dans n'importe quelle app. Rien ne part sur Internet.

## Télécharger

- **Mac** (puce Apple M1 ou plus récente, macOS 14+) : [Sovo-Mac.zip](https://github.com/Yoanmot/sovo/releases/latest/download/Sovo-Mac.zip). Touche **Fn**.
- **Windows** (10 ou 11, 64 bits) : [Sovo-Windows.zip](https://github.com/Yoanmot/sovo/releases/latest/download/Sovo-Windows.zip). Touche **AltGr**.

Prévois environ 2 Go de libre : au premier lancement, Sovo télécharge son modèle de transcription (Whisper Medium, 1,5 Go).

## Installer sur Windows

1. **Extraire.** Clic droit sur `Sovo-Windows.zip` > **Extraire tout...** Choisis un dossier qui ne bougera plus, par exemple `C:\Users\<ton nom>\Sovo` (évite Téléchargements, que tu risques de vider un jour).
2. **Lancer.** Ouvre le dossier `Sovo` et double-clique sur **Sovo.exe**. Ne sors pas `Sovo.exe` du dossier : il a besoin des fichiers à côté de lui.
3. **Passer l'écran bleu (SmartScreen).** « Windows a protégé votre ordinateur » : clique sur **Informations complémentaires**, puis **Exécuter quand même**. Windows ne te le redemandera plus pour cette version.
4. **Visual C++ (si une fenêtre en parle).** Clique **OK** et accepte l'autorisation de Windows : l'installeur officiel de Microsoft est déjà dans le dossier, ça prend une minute.
5. **Premier lancement.** L'icône Sovo apparaît près de l'horloge (sinon, sous la petite flèche **^**). Sovo télécharge son modèle (1,5 Go) : clique sur l'icône pour voir le pourcentage, une notification te prévient quand c'est prêt. Ensuite, ça marche sans Internet.
6. **Micro (si Sovo n'entend rien).** Paramètres Windows > Confidentialité et sécurité > Microphone : active **Accès au microphone**, **Autoriser les applications à accéder à votre microphone**, et plus bas **Autoriser les applications de bureau à accéder à votre microphone**. Réessaie, pas besoin de relancer Sovo.
7. **Dicter.** Maintiens **AltGr**, parle, relâche. AltGr + une autre touche marche comme avant (@, #, €). Tu peux choisir Alt gauche dans les réglages.

### Si l'app est bloquée par le « Contrôle intelligent des applications »

Sovo est gratuit et n'est pas signé par un éditeur payant. Sur certains PC Windows 11, le Contrôle intelligent des applications le bloque sans proposer de bouton pour passer outre. Si tu veux vraiment Sovo, désactive cette protection :

Sécurité Windows > **Contrôle des applications et du navigateur** > **Paramètres du Contrôle intelligent des applications** > **Désactivé**.

À savoir avant : sur les versions récentes de Windows 11 (25H2 à jour), tu peux la réactiver plus tard. Sur les versions plus anciennes, la réactiver demande de réinitialiser Windows. Vérifie ta version dans Paramètres > Système > Informations. Relance ensuite `Sovo.exe`.

## Installer sur Mac

1. **Installer.** Double-clique sur `Sovo-Mac.zip`, puis glisse `Sovo.app` dans **Applications**.
2. **Ouvrir.** Double-clique sur Sovo. macOS dit qu'il ne peut pas vérifier l'app : clique **Terminé**. Puis Réglages Système > **Confidentialité et sécurité**, tout en bas : **Ouvrir quand même**, et confirme avec ton mot de passe.
3. **Autorisations.** Dans Réglages Système > Confidentialité et sécurité : **Accessibilité** et **Surveillance de l'entrée**, active Sovo ; **Microphone**, clique **Autoriser**. Quitte Sovo (icône en haut de l'écran > Quitter) et relance-le.
4. **Touche Fn.** Réglages Système > **Clavier** > « Appuyer sur la touche 🌐 pour » > **Ne rien faire**.
5. **Premier lancement.** Sovo télécharge son modèle (1,5 Go) et le prépare pour ta puce : compte 5 à 10 minutes. Ensuite, c'est instantané et ça marche sans Internet.
6. **Dicter.** Maintiens **Fn**, parle, relâche.

## Notices complètes

- [Notice Mac](INSTALLER-MAC.md)
- [Notice Windows](INSTALLER-WINDOWS.md) (réglages, journal en cas de souci, désinstallation)
