# DPS meter Aion 2

Un DPS meter fait maison pour Aion 2 : dégâts et soins de ton groupe en direct, historique des
combats, résumé à coller sur Discord.

**[⬇ Télécharger la dernière version](https://github.com/Mitolius/aion2-dps-meter-releases/releases/latest)** (fichier `DPS-meter-Aion2.exe`)

## Installation

Rien à installer : pas de Python, pas de Npcap.

1. Dans le jeu, mets l'affichage en **plein écran fenêtré** (sinon la fenêtre du meter ne peut
   pas s'afficher par-dessus le jeu).
2. Lance `DPS-meter-Aion2.exe` **avant d'entrer dans une zone**, et accepte la demande des
   droits administrateur (nécessaires pour lire le trafic du jeu).
3. Si Windows affiche « Windows a protégé votre ordinateur » : **Informations complémentaires**
   puis **Exécuter quand même** (l'exe n'est pas signé par un éditeur connu).

Au premier lancement, le meter ajoute au pare-feu Windows une règle « DPS meter Aion 2 -
reception jeu » : elle l'autorise uniquement à **recevoir** les paquets venant du port du jeu.

## Mises à jour

Au lancement, le meter regarde s'il existe une version plus récente sur cette page. Si oui, la
barre du bas l'indique : un clic la télécharge, vérifie son empreinte SHA-256 et redémarre le
meter. L'historique et les réglages sont conservés (`%APPDATA%\Aion2 DPS meter\`).

## Signaler un problème

Dans le menu ☰ du meter :
1. **● Enregistrer le trafic du jeu**, refais le combat qui pose problème, puis arrête
   l'enregistrement (facultatif, mais ça aide beaucoup) ;
2. **Créer un rapport de diagnostic** : un fichier `.zip` apparaît sur ton Bureau, envoie-le
   sur Discord.

L'enregistrement contient tout ce que le jeu t'envoie, chat compris : ne l'envoie qu'à
quelqu'un de confiance. Rien n'est envoyé automatiquement.

## Confidentialité

- Le meter lit le trafic du jeu **sur ton PC** et n'envoie rien : pas de serveur, pas de
  classement en ligne, pas de capture d'écran.
- Sa seule connexion à internet est la vérification des mises à jour sur cette page GitHub.
  Pour la couper : `"check_updates": false` dans `%APPDATA%\Aion2 DPS meter\settings.json`.

Outil non officiel, sans lien avec NCSOFT. À utiliser à tes risques.
