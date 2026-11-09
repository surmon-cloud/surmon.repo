# surmon.repo
Mon homelab et le blog qui le raconte : IA locale, sauvegardes rejouées, automatisation, logiciels libres.

surmon.cloud est le carnet de bord d'un cloud personnel. J'y écris ce que j'apprends en faisant tourner mes propres services : l'IA en local, les sauvegardes qu'on rejoue pour de vrai, l'automatisation, et la souveraineté de ses données.

Ce dépôt rassemble les notes et les outils que j'en tire, quand ils peuvent servir à d'autres.

Les principes
Le local d'abord. Un service tourne chez moi avant d'aller chez un tiers.
Les logiciels libres. Chaque brique du labo est libre ou open source.
Une sauvegarde n'existe que restaurée. Les restaurations sont rejouées et datées.
L'état réel fait foi. Une doc dit ce qui était vrai quand on l'a écrite ; le journal et le service disent ce qui est vrai maintenant.
Le labo en quelques chiffres
Services	environ 130 conteneurs Docker derrière un seul reverse proxy
Machines	un serveur principal, un NAS, un VPS en DMZ, une machine de calcul GPU
IA locale	un modèle de 35 milliards de paramètres, plus l'embedding et le reranking, sur le serveur
Sauvegardes	chaque nuit, avec une alerte par source si une copie a plus de 30 heures
Les briques
Conteneurs et réseau : Docker Compose, Caddy, CrowdSec, NetBird.
IA locale : llama.cpp (llama-server) avec des modèles Qwen, LiteLLM, Qdrant.
Automatisation : n8n.
Sauvegardes : Kopia, instantanés btrfs immuables, dumps des bases vérifiés avant chaque copie.
Secrets : Infisical, Vaultwarden.
Supervision : Uptime Kuma.
Publication : Ghost, pour le blog.
À lire sur le blog
Yandex, Google : la vie numérique tient dans quelques bâtiments
L'IA ne vous rend pas expert : elle amplifie votre savoir
Tous les articles : surmon.cloud.

Ce que ce dépôt ne contient pas
Aucune configuration de production, aucun secret, aucune adresse interne. Le labo vit dans un dépôt privé ; ce qui arrive ici est relu et nettoyé avant d'être publié.

Licence
Les textes sont sous licence CC BY-SA 4.0. Vous pouvez les reprendre et les adapter, en citant surmon.cloud et en partageant sous la même licence. Le code qui arrivera ici portera sa propre licence, libre elle aussi.

Houari Bengana · surmon.cloud

