# Bot Discord

Mon but initial avec ce bot, était de le réaliser pour moi et mes amis. Le projet a évolué pour devenir un projet permettant à n'importe qui de déployer un bot d'administration facilement.

Il suffit seulement de créer un fichier de configuration et d'installer les modules node nécessaires, comme mentionné dans le readme.

## Fonctionalitées

Le bot utilise la fonctionnalité majeure de la version 10 de l'API de Discord : les "Slash commands".
Ces commandes sont plus intuitives à utiliser car leurs syntaxes sont détaillées lors de l'écriture de celles-ci, contrairement aux anciennes commandes dont il fallait quasiment apprendre leur syntaxes si on ne veut pas lire la documentation du bot à chaque fois qu'on veut l'utiliser


<img src="../../images/Encart discord.png" alt="Encart des 'Slash commands' de discord" width="75%">

Les commandes sont définies dans le code du bot, dont l'affichage est géré par Discord après les avoir déployés.

<img src="..\..\images\Syntaxe.png" alt="Exemple d\'aide syntaxique. Le type d'argument a donner est défini dans le code de la commande" width="75%">

Voici l'aide syntaxique proposée par Discord. Le type d'argument à donner est défini dans le code de la commande

## Commandes

- Administration
    - Ban (Bannit un utilisateur du serveur)
    - Kick (Éjecte un utilisateur du serveur)
    - Timeout (Retire temporairement le droit d'envoyer des messages et de rejoindre un salon vocal d'un utilisateur)
- Informations utilisateurs/Serveur
    - User (Renvoie les informations d'un utilisateur)
    - Serveur (Renvoie les informations sur le serveur actuel)
    - Ping (Renvoie pong, ainsi que la latence du bot)
- Autres
    - Poll (Crée un sondage, auquel les utilisateurs peuvent répondre avec les réactions)
    - 8ball (Renvoie une prédiction à propos d'une action)
    - Meme (Renvoie un meme aléatoire récupéré depuis Reddit)

D'autres commandes et fonctionnalités arriverons bientôt, au fur et a mesure que j'effectue la migration depuis la version 8 de l'API

Les ressources que j'ai utilisées sont le guide officiel de la librairie Discord.js ainsi que sa documentation.  
Lien du repository : <a href="https://github.com/loulou310/bot-framework">Lien</a>