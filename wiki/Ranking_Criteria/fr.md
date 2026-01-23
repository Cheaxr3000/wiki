'# Critère de classement de Titanic!

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
		- Les 'sliders' à Courbe Parfaite sont le genre de 'sliders' qui sont crée quand il y a 3 points de controle dans les clients à partir de 20121106 ou après (i'm not even sure what was said in english :sob:)
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

## Mode-specific

*Please refer to the osu! wiki for the full game-mode sepecific ranking criterias!*

### osu!

- **No offscreen objects in 4:3 aspect ratios.**
- **[The Auto mod](https://osu.ppy.sh/wiki/images/Ranking_criteria/Simplified_ranking_criteria/wiki/Gameplay/Game_modifier/Auto) must achieve bonus score on spinners.** They're too short otherwise.
- **Use at least two combo colors.**

### osu!taiko

- **Avoid covering essential parts of the background with the taiko playfield.** You can edit the vertical offset of the background in the [`.osu` file](/wiki/Client/File_formats/osu_(file_format)).
- **Avoid rapid [kiai](/wiki/Gameplay/Kiai_time) toggles.**
- **On rhythms that are 1/4 or faster, use big notes only at the end of patterns.**
- **Avoid slider velocity changes on lower difficulties.**
- **Each difficulty should follow its respective break length guidelines:**

| Difficulty | Break | Chain length |
| ---------: | :---: | :----------: |
| **Kantan** | ![3/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/kantan.png "3/1") | Break needed every 32–36 beats |
| **Futsuu** | ![2/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/futsuu.png "2/1") | Break needed every 32–36 beats |
| **Muzukashii** (option 1) | ![3/2](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/muzu1.png "3/2") | Break needed every 16–20 beats |
| **Muzukashii** (option 2) | ![3 consecutive 1/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/muzu2.png "3 consecutive 1/1") | Break needed every 16–20 beats |
| **Oni** | ![1/1](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Ranking_Criteria/img/oni.png "1/1") | Break needed every 16–20 beats |

### osu!catch

- **[The Auto mod](https://osu.ppy.sh/wiki/Gameplay/Game_modifier/Auto) must be able to SS your map.**
- **Avoid [dashes](https://osu.ppy.sh/wiki/Gameplay/Dash) and [hyperdashes](https://osu.ppy.sh/wiki/Gameplay/Hyperdash) that lead to the edges of the screen.** Placements between x = 16 and x = 496 are okay.
- **[Overall difficulty](https://osu.ppy.sh/wiki/Beatmap/Overall_difficulty) should match [approach rate](https://osu.ppy.sh/wiki/Beatmap/Approach_rate).**

### osu!mania

- **[Spread](#spread) rules apply to each key mode or [playstyle](https://osu.ppy.sh/wiki/Ranking_criteria/osu!mania#common-terms) separately.** For example, if you have 4K and 7K difficulties, you need two difficulty spreads.
- **Beatmaps can only use 4–10, 12, 14, 16, or 18 keys.** Key modes over 10 keys must use [certain playstyles](https://osu.ppy.sh/wiki/Beatmapping/osu!mania_10K_plus_playstyles).
- **No column can be left empty.**
- **No more than 6 notes can be pressed at the same time in Insane or lower difficulties.**
- **Difficulties using an [N+1 playstyle](https://osu.ppy.sh/wiki/Ranking_criteria/osu!mania#common-terms) must enable the `Use special style (N+1 style) for mania` toggle.**

## Song interpretation

*Note: This section is based on subjective mapping views, not the ranking criteria.*

**Every element of a map should represent the song.**

This principle sounds simple, but it might be the most controversial part of ranking a map! There's no *correct way* to interpret a song, so each individual's interpretation varies, and the [Beatmap Approval Team](https://osu.titanic.sh/g/3) determine if your interpretation is valid for Ranked status. Every BAT member may have a different opinion on this subject, but it's a good idea to follow older mapping styles.

These pointers may also lead you in the right direction:

- **Correlate map and song intensity.**
  - **Rhythm:** Intense parts have more rhythm density than calm parts.
  - **Spacing:** Intense parts have higher jump distance than calm parts.
  - **Slider velocity:** Intense parts have faster sliders than calm parts.
  - **Design:** Intense parts have more complex object composition than calm parts.
  - When the song gradually increases or decreases intensity, show a gradual progression of any elements above.
- **Show song variation through contrast.**
  - Establish some core ideas for your mapping choices.
  - When the song enters a new section, shift those mapping ideas according to how different the song feels.
  - If a specific sound only occurs once or twice in a song, make it stand out by clearly deviating from your usual mapping choices.
- **Be consistent (within reason).**
  - When a song repeats itself, it makes sense to repeat your map too.
  - Copying and pasting part of your map can be pretty boring though, so when a song repeats, vary your map in ways that don't drastically change how you previously interpreted the song.
- **Ask how your objects fit into the *"every element of a map should represent the song"* principle.**
  - **Example 1:** "How does this object represent the sound it aligns with?"
  - **Example 2:** "How does this section of objects follow the general mood of this section of the song?"
- **Consider how other people will interpret your map.** If your way of interpreting the song isn't clear, it'll feel like your map doesn't follow the song!
