# Critère de classement de Titanic!

Ces ensemble de critère de classement établisses les règles et directivrs que les 'beatmaps' doivent suivre afin de progresser dans la procédure de classement de 'beatmap'.
Les critère de classement suivent en grande partie la version [original](https://osu.ppy.sh/wiki/en/Ranking_criteria) avec quelque petits changement.

Les règles ont aussi été simplifié pour donner au mappeurs une perspective clair sur ce qui est requis pour crée une 'beatmap' classable. Les sections qui ne sont pas traité dans ce document devront être réferencer depuis [ici](https://osu.ppy.sh/wiki/en/Ranking_criteria).

[TOC]

Pour qu'une 'beatmap' soit classée, elle doit suivre ce critère de classement, ainsi qu'avoir été revue par au moins **2 [membres indépendent du BAT](https://osu.titanic.sh/g/3)**, plus un pour chaque mode de jeux. Cela veut dire, qu'un BAT ne peux pas approuvé leur propre map, et que les 'beatmaps' avec plusieurs modes de jeux requièrent aussi une approbation d'autre membres du BAT de ce mode de jeux.
This criteria may change in the future, due to increasing map requests and BAT members.
Ces critères pourrait changer dans le futur, due à la requête de map et membres du BAT montante. (unsure, seems weird)

# 'Beatmap'

- **Soyez sûre que tout dans la 'beatmap' est claire, en termes de la "[content usage permissions](https://osu.ppy.sh/wiki/Rules/Content_usage_permissions#artist-permissions) (cette page n'existe pas en français)."**
- **Les difficultés doivent faire au moins 30 secondes de long.**
- **La 'beatmap' devrait utilisé au plus possible et raisonablement le fichier audio.** Si vous avez une grande proportion non mappé, considérez de coupez la musique.
- **Les 'beatmaps' ne doivent pas utiliser des paramètres décimale.** (c.-à-d. AR9.3 -> 9)
- **Maps must not use any backgrounds, music, or objects made with the use of generative tooling.**
- **Les 'beatmaps' ne doivent pas utlisé n'importe quelle arrière plan, musique, ou objets génerée via l'utilisation d'un outil géneratif.** (unsure)

### Spread

- **Les 'mapsets' doivent avoir un 'drain time' total de au moins 90 secondes (1 minute et 30 secondes).**
- **Les noms de difficultés doivent avoir une progression.**
	- Easy -> Normal -> Hard -> Insane -> Expert, est la progression par défaut.
	- Une progression logique comme Seed -> Sprout -> Tree sont autorisée aussi.
	- **Exception:** La difficulté la plus dure peut utilisée un nom personnalisé, comme Normal -> Hard -> *Melancholy*
- **Ne sauter pas de difficultés.** Par example, si vous avez des difficultées Normal et Insane, vous avez besoin d'une Hard aussi
- **Un [meppeur invité](https://osu.ppy.sh/wiki/Beatmap/Guest_difficulty) ne peut pas créer plus de difficulté que l'[hôte](https://osu.ppy.sh/wiki/Beatmap/Beatmap_host).**

### Utilisation des 'Sliders'

- **L'utilisation de 'Sliders' à Courbe Parfaite est fortement déconseillé.**
  - Perfect Curve sliders are the type of sliders creating when a slider has 3 control points in clients b20121106 or later
		- Les 'sliders' à Courbe Parfaite sont le genre de 'sliders' qui sont crée quand il y a 3 points de controle dans les clients à partir de b20121106 et après (i'm not even sure what was said in english :sob:)
  - ![Example of Slider Curve Types](https://github.com/user-attachments/assets/ac50d9f8-ceb2-4fbe-9420-9cd1eba9de60)
  - Ces 'sliders' sont convertis en sliders Catmull sur les vieux clients. Cela cause la forme des 'sliders' a différencié grandement, créeant une différences de gameplay sur ces clients. Pour éviter ces problèmes, nous recommendos vivement aux 'mappeurs' d'utilisée n'importe qu'elle autre types de courbe de 'slider'. Dans l'image si-dessus, vous pouvez voir comment des squelletes de sliders identiques crée des chemin différent sur chaque type de courbure.
  - **Exception:** Les 'slider' à courbure parfaite avec très peu de courbe seront générallement bien converti, mais pour être sûre, nous recommendons de ne pas utilisé des courbes parfaite.
  - For information on how to avoid using Perfect Curve, [check out this forum post](https://osu.titanic.sh/forum/13/t/731/)!
  - Pour plus d'information sur comment évité l'utilisation de 'slider' à Courbe Parfaite, [regardez ce fil de discussion](https://osu.titanic.sh/forum/13/t/731/)!

### Visuels

  - **Évitez d'utilisez des couleurs de combo, bordure de 'sliders' ou 'hitcircleoverlays' avec ~50 luminosité ou en bas.** Les couleurs sombre comme cela impact la lisibilité des cercles d'approches avec un assombrissement de fond assez haut, et les autres éléments ne serves partiellement plus leurs fonctions de bordures.
  - **Évitez d'utilisez des couleurs de combo, et chemin de sliders avec ~220 de luminosité ou plus haut pendant les temps de kiai.** Cela crée des pulsasions brillantes qui peuvent être désagréable aux yeux.

### Hitsounds

- **Les 'beatmaps' doivent être ['hitsounded'](https://osu.ppy.sh/wiki/Beatmapping/Hitsound),** a l'éxception des 'beatmaps' osu!mania.
- **Chaque objet clickable doivent émettre un retour sonore audible.**

### Timing

- **Les maps doivent être correcement rhytmé.** Cela inclue le BPM et la signature des temps.
- **Chaque difficultés doivent utilisées le même timing.**
- **Ne changez pas les timing pour ajuster la vélocité des 'sliders'.**
- **Les objets doivent être alignés sur les tiques du rhytme de la musique.**
- **Seulement un object est autorisée par tiques,** à l'exception des 'beatmaps' d'osu!mania.
- **Un temps d'avancement (appelez lead-in time) doit être ajoutez manuellement si le premier objet est placez après 1500ms**

## Metadonnées

- **Les metadonnées doivent être fidèle.**
  - Utilisez une [source primaire de métadonnées](https://osu.ppy.sh/wiki/Beatmap/Primary_metadata_source).
  - Si la musique a une 'beatmap' classé ou 'Loved', utilisez les metadonnées de cet 'beatmap' à part si elle sont clairement mauvaise.
- **Utilisez [la méthode Hepburn de romanisation](https://en.wikipedia.org/wiki/Hepburn_romanization#Features) pour les mots Japonais.**

### Tags

- **Ajoutez le nom d'utilisateur de n'importe qui ayant contribuée à la 'beatmap'.** Cela n'inclue pas les moddeurs.
- **Ajoutez le [genre et la langue](https://osu.ppy.sh/wiki/Beatmap/Genre_and_language) de la musique.**
- **Ajoutez `featured artist` si la musique est dans le [catalogue de Featurd Artists](https://osu.ppy.sh/beatmaps/artists).**
- **Les autres tags doivent être pertinant à la musique/'beatmap'.**

### Titre

- **Les musiques qui ont été raccourcis pour la Télévision doivent avoir `(TV Size)`.**
- **Remplacez les marqueurs de version d'un jeu avec `(Game Ver.)`.**
- **Remplacez les marqeurs de versions racourcis avec `(Short Ver.)`.**
- **Utilisez `(Cut Ver.)` pour indiquer une coupure non officiel d'une musique.**
- **Utilisez `(Extended Edit)` pour indinquer une extension non officiel d'une musique.**
- **Utilisez `(Sped Up Ver.)` pour indiquer une augmentation du tempo non officiel de la usique.** Pour certains genres, `(Nightcore Mix)` est une alternative acceptable.

### Source

- **Utilisez le champ de Source si la musique vient d'une autre source de mediatique, comme une jeu, filme ou évennement.**

## Fichiers

- **N'utilisez pas de contenu inappropié.** Voir [règles générale relative au contenu des musiques](https://osu.ppy.sh/wiki/Rules/Song_content_rules) et [considerations relatives au contenue visuel](https://osu.ppy.sh/wiki/Rules/Visual_content_considerations).
- **N'incluez pas des fichier inutliser dans le fichier de la map.**

### Musique

- **Utilisez des fichiers de formats `.mp3` ou `.ogg`.**
  - Au plus 192 kbps pour les fichier `.mp3`.
  - Au plus 208 kbps pour les fichier `.ogg`. 
  - Au moins 128 kbps pour n'importe quelle type de fichier.
- **Un fihier de musique doit être utilisé pour toute les difficultées.**
- **Mettez un point d'aperçue consistent pour toute les difficultées.**

### Hitsounds

- **Hitsound files must be at least 25 ms long and use `.wav` or `.ogg` file formats.**
- **Les fichiers de hitsounds doivent faire au moins 25 ms de long et utilisez les formats de fichier `.wav` ou `.ogg`.**
  - N'utilisez pas `.mp3`
  - **Exception:** Utilisez [ce fichier](https://up.ppy.sh/files/blank.wav) for silent hitsounds.
- **Les hitsounds ne doivent pas être [en retard](https://osu.ppy.sh/wiki/images/Ranking_criteria/Simplified_ranking_criteria/img/delay.png).**

### Arrière-plan

- **Chaque difficultées doivent avoir un arrière-plan se conformant aux principes suivants:**
  - **Largeur minimum:** 160 px
  - **Hauteur minimum:** 120 px
  - **Largeur maximum:** 2560 px
  - **Hauteur maximum:** 1440 px
  - **Taille de fichier maximum:** 2.5 MB
- **Mettez un lien vers la source de l'arrière-plan de la 'beatmaps' dans la description.**

### Vidéo

- **Les vidéos doivent se confomées aux principes suivants:**
  - **Résolution maximum de la vidéo:** 1280x720
  - **Encodage vidéo:** H.264
- **La piste audio doit être enlever du fichier video.**

## Spécific aux modes

*Referrez vous s'il-vous-plaît au wiki de osu! pour le les critères de rankigns entier sur les game-modes specifiques!*

### osu!

- **Aucun objet hors de l'écran en proportions 4:3.**
- **Le [mod auto](https://osu.ppy.sh/wiki/images/Ranking_criteria/Simplified_ranking_criteria/wiki/Gameplay/Game_modifier/Auto) doit faire du score bonus sur les spinners.** Sinon ils sont trop court.
- **Utilisez aux moins deux couleurs de combo.**

### osu!taiko

- **Évitez de couvrir des parti essentiel de l'arrière ploan avec le terrain de jeu de taiko.** Vous pouvez éditez l'offset vertical du fond dans le [fichier `.osu`](/wiki/Client/File_formats/osu_(file_format)).
- **Évitez des activations de [kiai](/wiki/Gameplay/Kiai_time) rapide.**
- **Sur les rythmes qui sont en 1/4 ou plus rapide, utilisez uniquement des grosse notes à la fin des patternes.**
- **Évitez d'utilisez des changement de vélocité de slider sur les difficultés plus basses.**
- **Chaque difficultées doivent suivrent leur longueur de pause respectives:**

| Difficulty | Break | Chain length |
| ---------: | :---: | :----------: |
| **Kantan** | ![3/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/kantan.png "3/1") | Pause néccessité chaque 32–36 beats |
| **Futsuu** | ![2/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/futsuu.png "2/1") | Pause néccessité chaque 32–36 beats |
| **Muzukashii** (option 1) | ![3/2](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/muzu1.png "3/2") | Pause néccessité chaque 16–20 beats |
| **Muzukashii** (option 2) | ![3 consecutive 1/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/muzu2.png "3 consecutive 1/1") | Pause néccessité chaque 16–20 beats |
| **Oni** | ![1/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/oni.png "1/1") | Pause néccessité chaque 16–20 beats |

### osu!catch

- **[Le mod Auto](https://osu.ppy.sh/wiki/Gameplay/Game_modifier/Auto) doit être capable de SS votre map.**
- **Évitez des [dashes](https://osu.ppy.sh/wiki/Gameplay/Dash) et [hyperdashes](https://osu.ppy.sh/wiki/Gameplay/Hyperdash) qui amène au bords de l'écran.** Des placements entre x = 16 et x = 496 sont acceptable.
- **[L'overall difficulty](https://osu.ppy.sh/wiki/Beatmap/Overall_difficulty) devrait correspondre à l'[approach rate](https://osu.ppy.sh/wiki/Beatmap/Approach_rate).**

### osu!mania

- **Les règles de [spread](#spread) s'applique à chaque mode de touches ou [playstyle](https://osu.ppy.sh/wiki/Ranking_criteria/osu!mania#common-terms) separately.** Par exemple, si vous avez des difficultés en 4K et en 7K, vous avez besoin de deux spread de difficultées..
- **Les 'beatmaps' peuvent n'utilisez que 4-10, 12, 14, 16, ou 18 touches.** Les mode de touches au dessus de 10 touches doivent utilisez [certains playstyles](https://osu.ppy.sh/wiki/Beatmapping/osu!mania_10K_plus_playstyles).
- **Aucune colonnes ne peut être laisser vide.**
- **Pas plus de 6 notes ne doivent être appuyer au même moment sur des difficultées Insane ou en bas.**
- **Les difficultées utilisant le [playstyle N+1](https://osu.ppy.sh/wiki/Ranking_criteria/osu!mania#common-terms) doivent activées l'option `Use special style (N+1 style) for mania`.**

## Interprétation de la musique

*Note: Cette section est basée sur les vus de 'mapping' subjectives, et non critère de classement.*

**Chaque élement d'une 'beatmap' devrait représenter la musique.**

Ce principe à l'air simple, mais peut être la partie la plus controversé de classé une 'beatmap'! Il n'y a aucune *façon correcte* d'interprété une musique, donc chaque interprétation individuel varie, et la [Beatmap Approval Team](https://osu.titanic.sh/g/3) determine si votre interpretation est valide pour être classé. Chaque membre du BAT peuvent avoir une opinion différente sur ce sujet, mais c'est une bonne idée de suivre les traces de style de 'mapping' plus vieux.

Ces indications peuvent également vous mettre sur la bonne direction:

- **Correlez l'intensitez de la 'beatmap' et la musique.**
  - **Rhythme:** Les partie intense devrait être plus rythmiquement dense que les partie calme.
  - **Espacement:** Les parties intense devrait avoir une distance de 'jump' plus haute que les parties calme.
  - **Vélocité des 'sliders':** Les parties intense devrait avoir de 'sliders' plus rapide que dans les parties calme.
  - **Design:** Intense parts have more complex object composition than calm parts.
  - **Design:** Les parties intense devrait avoir des compositions d'objet plus complexe que les parties calme. (unsure)
  - Quand la musique monte ou descend graduellement en intensité, montrez une progression graduelle de n'importe quelle des éléments ci-dessus.
- **Montrez la variation musical à travers le contrast.**
  - Etablissez des d'idées principal pour vos choix de 'mapping'.
  - Quand la musique entre dans une nouvelle section, changez ces idées de 'mapping' en accord avec le ressenti différent de la musique.
  - Si un son spécifique se produit une ou deux fois dans une musique, faite le se démarquer en déviant clairement de vos chois de 'mapping' habituel.
- **Soyez consistent (dans la limite du raisonable).**
  - Quand une musique se répète, cela fait du sens de répeter votre 'beatmap' aussi.
  - Cependant copier et coller des parties de votre 'beatmap' peut être assez ennuyant, donc quand une musique se répète, variés votre 'beatmap' de façon à ce que cela ne change pas drastiquement de comment vous aviez interpréter la musique avant.
- **Demandez comment vos objets rentre dans le principe de *"chaque élément d'une 'beatmap' devrait représenter la musique"*.**
  - **Exemple 1:** "Comment est-ce que cet objet représente le song avec lequel il est aligné?"
  - **Exemple 2:** "Comment cette section d'objets suit l'humeur general se cette section de la musique?"
- **Considérez comment les autres personnes vont interpréter votre 'beatmap'.** Si votre manière d'interpréter la musique n'est pas clair, cela donnera l'impression que votre 'beatmap' ne suit pas la musique!
