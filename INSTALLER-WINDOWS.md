# Installer Sovo sur ton PC Windows

Sovo, c'est de la dictée vocale qui tourne entièrement sur ton PC. Tu maintiens la touche **AltGr**, tu parles, tu relâches : le texte s'écrit là où se trouve ton curseur (Chrome, Word, Bloc-notes, Discord, n'importe où). Rien ne part sur Internet.

**Avant de commencer, vérifie deux choses :**
- Windows 11 (ou Windows 10 à jour), version 64 bits.
- Environ 2 Go de libre sur le disque C: (le modèle de transcription pèse 1,5 Go).

## 1. Installer

1. Fais un clic droit sur `Sovo-Windows.zip` > **Extraire tout...**
2. Choisis un dossier qui ne bougera plus, par exemple `C:\Users\<ton nom>\Sovo` (évite le dossier Téléchargements, que tu risques de vider un jour). Sovo se relance tout seul au démarrage depuis cet endroit : si tu déplaces le dossier plus tard, relance Sovo une fois depuis le nouvel endroit et il se recale.
3. Ouvre le dossier `Sovo` et double-clique sur **Sovo.exe**. Ne sors pas `Sovo.exe` du dossier : il a besoin des autres fichiers à côté de lui.

## 2. Passer l'écran bleu de Windows (SmartScreen)

Sovo n'est pas signé par un éditeur payant, donc Windows affiche « Windows a protégé votre ordinateur » :

1. Clique sur **Informations complémentaires** (le petit lien sous le texte).
2. Clique sur **Exécuter quand même**.

Windows ne te le redemandera plus pour cette version.

**Si une fenêtre parle de « Visual C++ »** : c'est un composant gratuit de Microsoft dont Sovo a besoin, et ton PC ne l'a pas (ou en a une version trop ancienne). Clique **OK**, accepte l'autorisation de Windows, l'installation prend une minute, puis Sovo démarre. L'installeur officiel est déjà dans le dossier, rien à télécharger.

## 3. Premier lancement : patience

L'icône Sovo apparaît près de l'horloge, en bas à droite. Si tu ne la vois pas, clique sur la petite flèche **^** : elle est rangée là. Tu peux la glisser à côté de l'horloge pour l'avoir toujours sous les yeux.

La toute première fois, Sovo télécharge son modèle de transcription (**1,5 Go**). Compte quelques minutes avec une bonne connexion. Clique sur l'icône Sovo : le menu affiche « Téléchargement du modèle : xx % ». Une notification te prévient quand c'est prêt.

Ensuite, ça marche sans Internet.

## 4. Autoriser le micro (si Windows bloque)

À ta première dictée, si Sovo affiche « Sovo n'entend rien » ou « Windows bloque le micro » :

1. Ouvre **Paramètres Windows > Confidentialité et sécurité > Microphone**.
2. Active **Accès au microphone**.
3. Active **Autoriser les applications à accéder à votre microphone**.
4. Descends et active **Autoriser les applications de bureau à accéder à votre microphone** (Sovo est une application de bureau, il n'apparaît pas dans la liste du dessus).

Puis réessaie, pas besoin de relancer Sovo.

## 5. Utiliser

- **Maintiens AltGr** (la touche à droite de la barre d'espace), parle, **relâche**. Une petite pilule noire apparaît en bas de l'écran pendant que tu parles, puis un rond qui tourne pendant la transcription.
- Le texte se colle là où est ton curseur.
- **AltGr + une autre touche marche comme avant** : AltGr + à donne @, AltGr + " donne #, AltGr + E donne €. Dès que tu appuies sur une autre touche, Sovo annule la dictée et laisse passer ton caractère.
- Un appui très court sur AltGr ne déclenche rien : il faut le tenir le temps de parler.
- Ton presse-papier est préservé : ce que tu avais copié avant la dictée y est remis juste après.
- Sovo se lance tout seul quand tu allumes ton PC. Tu n'as plus à t'en occuper.

## 6. Réglages

Clique sur l'icône Sovo > **Réglages...** :

- **Touche** : AltGr (par défaut) ou Alt gauche. Avec Alt gauche, Alt+Tab et Alt+F4 marchent toujours normalement.
- **Langue parlée** : français par défaut.
- **Modèle** : Medium (par défaut, le plus précis) ou Small (plus rapide sur un PC sans carte graphique, moins précis). Small se télécharge depuis la même fenêtre (490 Mo).
- **Pilule** : l'afficher ou non pendant la dictée.
- **Lancer Sovo au démarrage de Windows**.

## 7. En cas de souci

Le journal de Sovo est ici : `%LOCALAPPDATA%\Sovo\Sovo.log`

Pour l'ouvrir : touche Windows + R, colle `%LOCALAPPDATA%\Sovo`, Entrée. Ou depuis Sovo : Réglages > **Ouvrir le dossier des journaux**.

Envoie ce fichier `Sovo.log` avec une phrase qui décrit ce qui s'est passé (et l'heure à peu près). Il ne contient pas d'audio, seulement les étapes et les textes dictés.

Pour quitter Sovo : clic sur l'icône > **Quitter**.

Pour le désinstaller : Réglages > décoche « Lancer Sovo au démarrage de Windows », quitte Sovo, puis supprime le dossier `Sovo` et le dossier `%LOCALAPPDATA%\Sovo` (qui contient le modèle).
