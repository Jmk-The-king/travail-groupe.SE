# travail-groupe.SE
compression et decompression des fichiers avec linux 

Bonjour et bienvenue sur ce guide readme pour la compression et la décompression avec la commande .tar de Linux Ubuntu. Dans ce guide, vous allez apprendre comment utiliser la commande .tar pour créer des archives compressées au format .tar.gz, .tar.bz2 ou .tar.xz, et comment les extraire. Vous allez également découvrir comment exclure des fichiers ou des dossiers de l'archivage, et comment choisir le logiciel de compression le plus adapté à vos besoins.

La commande .tar est un outil d'archivage qui permet de regrouper plusieurs fichiers ou dossiers en un seul fichier. Par défaut, une archive .tar n'est pas compressée. Il faut donc utiliser un logiciel de compression comme gzip, bzip2 ou xz pour réduire la taille de l'archive. Heureusement, la commande .tar gère la compression et peut créer une archive .tar et la compresser avec le logiciel de votre choix en une seule commande.

Voici les formats d'archives compressées que vous pouvez obtenir avec la commande .tar :

- .tar.gz : archive compressée avec gzip
- .tar.bz2 : archive compressée avec bzip2
- .tar.xz : archive compressée avec xz

Chaque logiciel de compression utilise un algorithme différent qui a ses avantages et ses inconvénients. Voici un résumé des performances de chaque logiciel :

- gzip : le plus rapide à extraire, mais le moins efficace en termes de taux de compression
- bzip2 : plus lent que gzip à extraire, mais plus efficace en termes de taux de compression
- xz : le plus lent à extraire, mais le plus efficace en termes de taux de compression

Le choix du logiciel de compression dépend donc de vos besoins et de vos contraintes. Si vous privilégiez la rapidité d'extraction, optez pour gzip. Si vous privilégiez le gain d'espace disque, optez pour xz. Si vous cherchez un compromis entre les deux, optez pour bzip2.

Pour créer une archive compressée avec la commande .tar, vous devez utiliser les options suivantes :

- -c : pour créer une archive
- -z : pour compresser avec gzip
- -j : pour compresser avec bzip2
- -J : pour compresser avec xz
- -v : pour afficher la progression dans le terminal (option facultative)
- -f : pour spécifier le nom du fichier d'archive

Par exemple, si vous voulez compresser le dossier /home/ubuntu/Documents avec gzip et créer une archive nommée documents.tar.gz, vous devez taper la commande suivante :

tar -czvf documents.tar.gz /home/ubuntu/Documents

Si vous voulez compresser le même dossier avec bzip2 et créer une archive nommée documents.tar.bz2, vous devez taper la commande suivante :

tar -cjvf documents.tar.bz2 /home/ubuntu/Documents

Si vous voulez compresser le même dossier avec xz et créer une archive nommée documents.tar.xz, vous devez taper la commande suivante :

tar -cJvf documents.tar.xz /home/ubuntu/Documents

Vous pouvez également compresser plusieurs fichiers ou dossiers à la fois en les listant après le nom du fichier d'archive. Par exemple, si vous voulez compresser les fichiers /home/ubuntu/Documents/notes.txt et /home/ubuntu/Documents/report.pdf avec gzip et créer une archive nommée files.tar.gz, vous devez taper la commande suivante :

tar -czvf files.tar.gz /home/ubuntu/Documents/notes.txt /home/ubuntu/Documents/report.pdf

Pour extraire une archive compressée avec la commande .tar, vous devez utiliser les options suivantes :

- -x : pour extraire une archive
- -z : pour décompresser avec gzip
- -j : pour décompresser avec bzip2
- -J : pour décompresser avec xz
- -v : pour afficher la progression dans le terminal (option facultative)
- -f : pour spécifier le nom du fichier d'archive

Par exemple, si vous voulez extraire l'archive documents.tar.gz dans le dossier courant, vous devez taper la commande suivante :

tar -xzvf documents.tar.gz

Si vous voulez extraire l'archive

Ce projet est réalisé par les étudiants membres du groupes N°1 dans le cadre du cours de système d'exploitation. 