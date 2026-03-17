# Différence d'Éditeur des Clients

[TOC]

### Écrie par Digitalfear117

Salut, je suis [Digitalfear117](https://osu.titanic.sh/u/809) et j'adore les vieux éditeurs. J'espère que les utilisateurs de titanic seront capable de mapper et classer des musiques utilisant n'importe quelle version disponible de osu! Ce guide décrit les fonctionalités dans l'ordre chronologique qu'elles ont été ajoutées. Il explique aussi comment le format de fichier. osu fonctionne, et ce que les valeurs font. Avec un peu de chance, par la fin de cette page vous saurez comment faire marcher des 'beatmap' moderne dans des vieux clients, et choisir le meilleur client pour faire vos 'beatmaps'!

J'ai omis certaine versions de cette liste ca je ne trouvait pas qu'ils avaient des changements assez signifiant avec eux. Si j'ai oublié quelque chose, n'hésitez pas a me contacter, ou contribuer a cette page!

### Téleverser des maps sur titanic

Pendant le developement de osu!, téleverser des maps à travers le ”Beatmap Submission System” (BSS) ont changé drastiquement. L'implementation du BSS sur titanic supporte tout les clients, même si il peut être un peu instable sur les plus vielle versions de osu!. Si vous rencontrez des problèmes, je reommanedrais d'utilisé mon client moddé b20130303, comme il vous autorises a outre-passer de mettre à jour la 'beatmap' avant le téleversement. Cela est particulièrement utile si vous voulez préservez la compabilité avec le client original que vous avez utiliser pour le 'mapping'!

# Versions de prélancement de osu! (v1)

Quelque versions de osu! existes qui prédate la beta publique officiel du jeu. Beacoupp des premières 'beatmaps' dans le jeu ont été fait pendant cette era de pré-lancement et ont été mis-à-jour par peppy aux .osu v3 puis classer.

## 07-27-2007

Cette version produit quelque une des 'beatmaps' les plus minimaliste de osu. Ce client manque la possibilité de faire quoique ce soit en dehors des cercles, même dans le .osu lla seul information est le 'hitobjects'

Voici un exemple d'un cercle dans ette version:

`96,64,8118,5,4`

## 07-29-2007

Le haut du fichier .osu de ce client enregistre maintenant le TEMPO et l'OFFSET. En dessous de cela est la donné du 'hit object'. Cette versio est très similaire à l'ancienne, mais maintenant les 'sliders' marche (généralement)! Quelque chose d'important à noter est que les têtes et corps de 'slider' doivent commencer à la même position, contrairement aux versions précedente de l'editeur. Le seul type de slider qui existe dans cette version est le type 'catmull'. Vu qu'il n'y a aucun autre type de courbe de 'slider', le. format de 'slider' est simplifier.

Voici un exemple d'ub 'slider' dans cette version:

`224,80,17118,2,0,224:80|336:32|360:153,1`

## 08-26-2007

Si vous voulez créer des nouvelles 'beatmaps' dans cette version, vous devez créer un fichier dans le réportoire "Songs", et à l'intérieur de ce fichier, vous devez avoirun fichier mp3 et .osu nommé identiquement. Créez ceux la avant d'ouvrir le jeu. Donc vous pouvez crédd un fichier appeler ˋMapˋ, et les fichier à l'interieure devront être ˋMap.mp3ˋ et ˋMap.osu

Cette version a 2 nouveaux tags dans le .osu, ˋSPEEDXˋ et ˋCUSTOMXˋ. SPEEDX est pour la vélocité des 'sliders'. CUSTOMX est pour le taux de tiques, mais ils n'ont pas l'air de fonctionné.

Voici un exemple d'en-tête du fichier .osu de cette version:

```
TEMPO 500
OFFSET 126
SPEEDX 1
CUSTOMX 1
```

# Versions de pré-lancement de osu! (v2)

Cette version du jeu est significativement plus utilisable que les autres versions de pré-lancement. Au jourd d'aujourd'hui nous avons qu'un seul client qui créer des .osu v2.

## 09-08-2007

Cette version à bien plus des informations néccessaire pour avoir une map lisible dans le osu! moderne. Les en-têtes pour séparé les données ont été implémenter. SPEEDX et CUSTOMX ont été renommé, le hachage audio est maintenant inclu dnas le fichier .osu, et vous pouvez  maintenant placé des 'sliders' 'beizer' en addition des 'sliders' lineéaire. Vous voyez comment il n'y a aucun moyen de changé les paramètres de difficultés. Et aussi comment il n'y a aucun moyen de nommé une difficulté pour l'instant.

Par contre je recommenderais que vous continuez d'utiliser le même nom de dossier et de fichier que dans les anciennes versions. Cela explique pourqoi certaine des premières 'beatmaps' sont tous aux paramètres ”par défault”, les utilisateurs n'avait pas encore le choix.

Il n'y a aucun .osu v2 de classé, les v3 sont les premières versions officiel.

Voici le format .osu de cette version:

```
osu file format v2

[General]
AudioFilename: audio.mp3
AudioHash: a37859a4a0919cd369a1612762cb0c38
SpeedMultiplier: 1
CustomMultiplier: 1

[Metadata]
Title:Dango Daikazoku (TV Size)
Artist:Chata
Creator:Digitalfear117

[Events]

[TimingPoints]
226,600

[HitObjects]
0,0,226,2,0,C|0:0|0:128,1,100
0,192,1426,2,0
```

# b53 à b144 (v3)

Here is the first public release of osu! These are the oldest maps that are fully compatible in modern osu!, so if you want to map in pre-historic versions of the game, this is the most featured, and would require the least amount of additional effort to get working on your part.
Voici la première sortie publique de osu! Ceux ce sont les 'beatmaps' les plus vielles qui sont entièrement compatible dans le osu! moderne, donc si vous voulez mapper dans une version pré-historique du jeu, elle la plus mise en avant et vous requierais le moins d'effort possible pour la fair marcher de votre côter. (unsure)

Des changements notable dans le .osu v3 inclu l'autorisation d'ajuster les paramètres de difficulté. Notez que aucun de ces paramètres ne peuvent être mis en nombre décimales, et que l'OD et l'AR sont combinés: 

```
[Difficulty]
HPDrainRate:6
CircleSize:4
OverallDifficulty:6 // OD and AR are combined
SliderMultiplier: 1.4
SliderTickRate: 2
```

Vous pouvez maintenant choisisr un échantillion pour vos hitsounds en dans ”General”:

```
[General]
SampleSet: None
```

Les images ou vidéos peuvent maintenant être ajouté, et elles commenceronts au début du tag d'”Events”:

```
[Events]
0,0,"katamari2.jpg" // Background
2,34350,47100 // Break
```

## b70 'sliders' linéaires
Entre b53 et B70, les 'sliders' linéaires ont été ajouté! Vous pouvez maintenant faire des 'sliders' qui ont un effet moderne des ligne rouges. En revanche, dans cette version, vous devez choisir si vous voulez l'entiereté du 'slider' d'être linéaire, ou entièrement style 'beizer', ou entièrement style 'catmull'.

# b162 à b222 (v4)

Cette mis-à-jour du format de fichier .osu offres de nouvelles fonctionnalités qui sont assez utile.

Vous pouvez maintenant mettre un temps de 'lead-in' à l'audio, et activez ou désactivez la fonctionnalité de déconte dans ”General”:

```
AudioLeadIn: 0
Countdown: 1
```

Les points de timing ont 3 nouvelles additions qui peuvent être ajouté:

```
[TimingPoints]
118,500.004999999999,4,0,1
``` 

 - 4 réfère aux signatures de temps. Presque toute les 'beatmaps' seront en 4/4
 - Ici 0 réfères aux échantillons. 0 est legacy et se met par défault au ”Normal”. 1 est la bonne manière de mettre l'échantillon ”Normal”, 2 est pour ”Soft”. Rappelez vous que l'échantillon ”Drum” n'existe pas encore
 - 1 réfère à si vous avez cochez un échantillon customisé ou non. Dans cette versio du jeu, il peux y avoir 1 seul échantillon customisé.

## b196 storyboarding

Ceci est l'une des premières version de osu! qui supporte le langage de script de storyboard. L'onglet ”Design” ne serait pas fait pendant plusieurs versions, mais si ça ne vous embête pas de le faire dans un éditeur de texte, la pluparts des fonctions simple marche dans cette version.

## b222 ajustement de volume d'hitsound

Cette mis-à-jour vous laissez customisez les volumes d'hitsounds ne n'importe qulle point de timing. Cela veut dire que les tag de volume d'hitsound dans "Timing Points" peuvent être entre 0 et 100. Seul le jeu moderne vous laisse descendre a 5%, et forcera n'importe quelle valeur en dessous a 5% quand jouer.

![Audio section of the Timing Setup panel in b222](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b222_timing_setup_audio.png)

Example de .osu pour les volume d'hitsound:

```
[TimingPoints]
118,500.004999999999,4,0,1,42
```
- 42 réfere au volume en % de l'hitsound

# b282 à b904 (v5)

The switch to .osu v5 seemed to happen on 2008-03-24, but we have no builds in between b222 and b282. .osu v5 evolved a significant amount during it's time, so much so, that .osu v5's made in the last version that created this file format won't even work correctly in the first version that made this format!
Le changement au .osu v5 a l'air d'avoir pris place le 03/24/2008, mais nous avons aucune versions entre b222 et b282. Le .osu v5 a significament évoluer pendant son temp, tellement que, le .osu v5 a été fait dans le dernière versions qui créer ce genre de fichier ne marcheras pas correctement dans le première version qui a fait ce format! (unsure)

Les premières versions qui utilisent le .osu V5 ne sont pas maoritairement différent de ce qui était arriver avant, on aurait dit que le changement majeur est que les 25ms d'offset ont été enlever des nouvelles maps en allant de l'avant du a un changement que peppy a fait le 23 Mars 2008. Ceci est de son journal de modification officiel:

`Realised my silence finding function WASN'T RUNNING! Fixed, and adjusted previous beatmaps to earn themselves a free 25ms offset.` (Traduction: `J'ai réaliser que ma fonction de recherche de silence NE TOURNAIT PAS! Réparer, et ajuster au anciennes beatmaps pour qu'elles gagnent 25ms d'offset gratuit.`)

Au moment on j'écris ceci, ceci est la version la plus vielle possible qui marche sur osu!titanic, en revnache, seul les testeurs sont autorisé à l'utilisé du au bugs qui existe dans le client. Je pense que c'est dommage, mais peut être qu'un jour cela peut être changer.

## b294 enlever les encres de 'slider' redondant sur les têtes de 'slider'

Jusqu'a ce moment, le premier point de tout les corps de 'slider' copier les coordonées de la tête du 'slider' , créant un lien codé en dur du début du corps de 'slider' et la tête. À partir de cette versions par contre, ce lien est fait automatiquement par le jeu, et plus écrie éxplicitement dans le fichier .osu. Cela veut dire que tout les 'sliders' fait sur cette version de osu! et après seront cassée sur les vieux clients, donc faite attention!

|       |.osu Définition de 'Slider'                                   |
|-------|--------------------------------------------------------------|
|Before:|<code>224,80,17142,2,0,B\|224:80\|336:32\|360:153,1,140</code>|
|After: |<code>224,80,17142,2,0,B\|336:32\|360:153,1,140</code>        |

## b337 ancres rouge

À partir de cette version, vous pouvez maintenant créer des ancres rouges sur les 3 types de 'slider' disponible!

![Red anchor examples on all 3 slider curve types](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b337_red_anchors.png)

Adding a red anchor to a Bezier allows you to have sharp straight turns, this could be useful in situations where you want one part of the slider to have a straight turn, but you want another part to have a curved turn. Catmull sliders produce a loop bulb effect on red anchors, where the player is forced to hold on the red anchor. This could be useful on some more gimmicky maps, or to really emphasize a sound on a slider. As a consequence of the bulb though, the slider will end up appearing shorter than the other curve types when the slider anchors are identical. Adding a red anchor to a Linear slider does not do anything noticeable to it. 
Ajouter une ancre rouge a slider 'Bezier' vous autorise a avoir une courbe serré, cela peut être utilse dans les situations ou vous voulez qu'une partie du 'slider' ai une courbe droite, mais que vous voulez une autre partie du slider d'avoir une courbe courbé. Les sliders ”Catmull” font une ampoule bouclé sur les ancres rouges, le joueur est forcé de tenir sur l'ancre rouge. Cela peut être utile pour des 'beatmaps' un plus centré sur de la 'gimmick', ou pour vraiment souligner un son sur un slider. En consequence de l'ampoule en revanche, le 'slider' apparaîtra plus petit que les autres types de courbures quand les slider sont identiques. Ajouter une ancre rouge a un slider 'Linéaire' ne fera pas de changement signifiant à celui-ci. (unsure)

Les ancres rouges marchent dans le .osu en copiant la même ancre de 'slider' deux fois. Si le jeu voit deux points de 'slider' identique il le traiterai comme une ancre rouge.

|             |.osu 'Slider' Ancre Rouge vs Ancre Blanche                   |
|-------------|-------------------------------------------------------------|
|Red Anchor:  |<code>32,32,85207,6,0,L\|128:32\|128:32\|128:160,1,210</code>|
|White Anchor:|<code>32,32,85207,6,0,L\|128:32\|128:160,1,210</code>        |

## b337 les options activés sont enregistrés pendant les sessions

Si vous appuyez sur le bouton du ”Distance Snap”, ou du ”Grid SNap”, le client enregistrera maintenant votre selection jusqu'a ce que vous fermez le jeu.

## b370 changer les types de courbature de 'slider' rapidement

In this build you can easily try out the different slider curve types by pressing **A** **S** or **D**.
Dans cettte version, vous pouvez facilement essayez les différents types de courbure de 'slider' en appuyant sur **A** **S** ou **D**.

|Touche|Action |
|---|-------|
|A  |Linéare |
|S  |Catmull|
|D  |Bezier |

![Example of the on screen popup for swapping between slider curve types](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b370_slider_curve_popup.gif)

Cela vous autorisent a expérimenté plus simplement avec différents types de courbure de slider sut un seul objet si vous voulez essayez d'autre moyen de souligner un sond sans avoit a aller dans *Option > Slider Curve Type* chaque fois que voulez changer de type.

## b370 Spécificité au Taiko

Ceci est la première version disponible qui peut faire des 'beatmaps' en taiko! Vous pouvez avtivre cela en allant dans *Song Setup (F4) -> Advanced* et cochez la case **Made for Taiko Mod** 

Vous pouvez voir si une map est faite pour osu! ou taiko en regardant le nouveau signale sous la section ”General” du .osu

```
[General]
Mode: 0
```
-  0 osu! standard
- 1 taiko
- 2 catch the beat (ne sera pas rajouté jusqu'a b504)
- 3 mania (ne sera pas rajouté jusqu'au alentours de osy! 2012 b20121030)

## b370 lien de selections dans l'éditeur peuvent être appuyez en chat.

Une fonctionalité incontrournable pour ceux qui mod par le IRC

![An example of clickable editor selection links over in-game chat](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b370_editor_selection_links.png)
## b370 chercher par affichage du temp

![GoTo Time popup for jumping to a specific time stamp](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b370_goto_time_popup.png)

Clicking on the time stamp at the bottom left allows you to go to any time in the map easily.
Appuyez sur l'horodatage en bas a gauche vous autorise a aller à n'importe quelle temps dans la map facilement. (unsure)

## b394a tags

Dans cette version, vous pouvez maintenant rajoutez des tags directement au .osu dans le ”Song Setup”. Ceci apparaitra sous la section ”Metadadta”: 

```
[Metadata]
Tags:Digitalfear117
```

## b394a Lignes rouge et pauses sur la bar de défilement

Avec cette version, vous pouvez facielemnt voir les lignes rouges et les pauses sur la bar de défilement. Celles-ci n'apparaissait pas sur la timiline en haut ou les notes sont, mais pas sur la bar de défillement jsusqu'a cette version

![Example of a red line and break on the timeline](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b394a_red_lines_breaks.png)

Ceci fait en sorte de voir les aspects de la map un peu pls facilement, comme cela vous pouvez voir les sections de la 'beatmaps' en bas

## b420 lignes héritées

À partir de cette version, les nouveau points de timing peuvent héritée du BPM du point de timing antérieur. Ceci est ce qui va se transformer en lignes vertes, mais pour l'instant, elles sont toujours rouges.

![b420 Timing Setup popup, showing off an interited timing point](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b420_timing_setup.png)

You can tell if a timing point is inherited in the .osu based on if the last flag in the timing point is a 1 or a 0.
Vous pouvez voir si un point de timing a héritée dans le .osu si le dernier signale du point de timing est un 1 ou un 0. (unsure)

```
[TimingPoints]
2055,600,4,2,0,65,0
2555,600,4,2,0,65,1
```

The last flag being 0 means inherited, and 1 means non inherited in this version, and for a decent amount of versions after this.
Le dernier signale étant 0 veut dire que cette ligne a héritée, et 1 veut dire qu'elle n'a pas héritéée dans cette version, et pour une bonne poignée de versions après celle-la. (unsure, that whole version is unsure)

## b452 hitsound de "clap"

Ceci est la toute première version ou vous pouvez utilisez les hitsounds "clap"! Cette version a un "clap" disponible dans les deux versions d'échantillons ("Normal" et "Soft").

![A screenshot of the clap hitsound button from b452](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b452_clap_hitsound_button.png)

Vous pouvez voir quelle hitsoud a été appliquer à un cercle en regardant le dernier signale dans le .osu:

`96,128,45555,1,2` 

- La valeur de 2 à la fin est l'hitsound

|Signale|Hitsound |
|----|---------|
|0   |Aucun    |
|2   |Whistle  |
|4   |Finish   |
|8   |Clap     |

Ces nombres sont combinés quand vous ajoutez plusieurs hitsound a un objet. Par exemple, 6 serait "Whistle" et "Finish".

Ceci est aussi vrai pour les 'sliders', si l'entiereté du corp du 'slider' a un hitsound d'ajouter, vous le verrez sur le dernier chiffre avanr le type de courbure de 'slider'.

`96,128,52155,2,6,B|96:256,1,100`

- Ici il est marqué 6, donc cela veut dire que c'est "Whistle" + "Finish".

## b452 hitsound de tête de slider, queue, et flèche de retour

This version brings another major milestone for hitsounding, you can now hitsound the head, tail, and reverse arrow of a slider individually. Prior to this build you could only hitsound the entire slider body. You can do this by clicking on the body part in the timeline at the top, or the object on the play field until the segment gets highlighted in black.
Cette version amène un autre grand pilier pour le hitsounding, vous pouvez maintenant mettre des hitsounds sur la tête, queue, et flèche de retour d'un slder individuellement. Avant cette version, vous pouvez seulement mettre un hitsound sur l'entièreté du corp du slider. Vous pouvez faire cela en cliquant sur l'élément du corp dans la timeline en haut, ou l'objet sur la grille de mapping jusqu'à ce que le segment soit surligné en noir. (unsure)

![An example of me selecting a reverse slider for hitsounding](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b452_reverse_slider_selection.png)

Voici un example en .osu d'un slider avec une flèche de retour ou l'etièreté du corp de slider à un hitsoud, et chaque parties du slider ont un hitsound individuel:

`96,160,61755,2,2,B|224:160,2,100,4|6|10`


Comparé avec l'exemple de 'slider' d'avant, il y a maintenant une virgule en plus après le 100, the 4 étant un hitsound sur la tête de 'slider'. Après le charactère tube il y a un hitsou d avec une valeur de 6 sur la flèche de retour, et après le prochain tube un hitsound d'une valeur de 10 a été appliquer sur la queu de 'slider'. Cela veut dire que l'entièreté du corps du 'slider' à un hitsound Whistle et Finish appliquer dessus, et que la queu de 'slider' a un hitsound de Whistle et Clap appliquer dessus.


### b452 est le premier client qui n'a pas slider casser sinle kiai a été ajouter à un point de timing!


## b497 changement de storyboard

Faire un storyboard dans b497 a été grandement réviser, ceci est le format qui sera supporté plus tard par les premières versions de la fenêtre de design en jeu dans b595b. Ce format n'est pas grandement différent de ce qu'il y a dans la version moderne de stable, mais il y a quelque petite choses a garder en tête, Vous n'avez peut-être pas une fenêtre de design dans cette version, mais les storyboards sont visible dans l'editeur. Si vous voulez rechargez votre SB après les change:ents, faites ˋCONTROLE + Lˋ. Assez embettant que c'est, cette versions de osu! supprimera n'importe quelle ligne qu'elle ne comprend pas. Donc soyez sur de gardez votre editeur de texte ouvert ou ayez des backups.

Voici quelque règles importantes à connaitre pour faire un storyboard manuel dans ce format:

- Les coordonnées X & Y ne peuvent jamais contenir de decimals ˋ320,227.5ˋ serait invalide, pas comme dans le jeu moderne.
- Les commandes d'Échelle (Scale) doivent avoir un début et une fin. ˋS,0,11892,15594,04ˋ est valide dans la version moderne de stable, mais il peut être adapté pour avoir une fin d'échelle de transformation, même si c'est la même valeur. ˋS,0,11892,15594,0.4,0.4ˋ est valide dans ce format
- Stable moderne utilise le formzt simple à lire "Name" pour tout les objets telle que ˋSprite,Foreground,Centre,ˋ pour le début de n'importe quelle objet dans le storyboard. Cette version attend de vous d'utiliser des valeurs numérique pour représenter ces choses. Donc pour mon 'Sprite' d'exemple il est considéré comme type ˋ4ˋ, 'Foreground' est considéré type ˋ3ˋ, 'Centre' est considéré comme de valeur ˋ1ˋ. ˋ4,3,1,"Storyboard\Lyrics\A1.png",320,200ˋ serait un format valide pour cette version.

![Any example of a storyboard loaded in b497](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b497_storyboard.png)
Voici un exemple valide de tag de storyboard dans un .osb:

```
4,3,1,"Storyboard\Lyrics\A4.png",320,200
 F,0,232715,232905,0,1
 S,0,232715,235563,0.4,0.4
 F,0,235373,235563,1,0
```

Voici un exemple valide de tag de storyboard dans un .osu:

```
4,3,1,"Storyboard\Lyrics\A4.png",320,200
 F,0,232715,232905,0,1
 S,0,232715,232715,235563,0.4,0.4
 F,0,235373,235563,1,0
```
Pour certaines raisons, le temps de départ pour la transition de taille doit être là deux fois.

### b504 est le dernier build à autorisée CS 0-10 sans aller éditer dans le .osu

## b595b fenêtre design (editeur de storyboard en jeu)

![A screenshot of the in game storyboard design tab](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b595b_design_tab.png)
Vous pouvez maintenant faire des storyboards directement dans le jeu!

## b595b ligne vertes

Les points de timing qui ne change que les choses en rapports abev les hitsounds sont maintenant désigné comme des lignes vertes! Seul les points de timing avec des changements de BPM (ou non alignée) seront reçu comme lignes rouge. Rejouissez vous, vous pouvez finallement savoir ce qu'est la fonction de chaque ligne!

Si vous essayez d'importer une map moderne avec vélocités de slider le jeu lira le changement de vélocité de slider en tant qu'un changement d'un multiplicateur du BPM à la place, donc cette version ne supporte pas véritablement les changement de vélocité de slider pour l'instant.

## b595b Ajustement de BPM

![A screenshot of the Timing section within Timing and Control Points popup menu](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b595b_bpm_adjustment.png)

Les options d'ajustement de BPM sont maintenant disponible dans le popup 'Timing and Control Points'! Ceci vous permez de changer le BPM par 0.5 ou 2.0 pour mieux soulignez les partie plus ou moins intenses d'une musique! Tout a propos de l'éditeur se rapporte au BPM par contre, doublez le BPM voudra dire que votre vélocité de slider est maintenant doubler, votre distance snap est maintenant doubler. Même si les valeurs du jeu montre les mêmes, ceci est le vrai résultat. Ceci est pareil dans le jeu moderne aussi.

## b595b additional sample set custom override
## b595b échantillon additionel remplacement custom (unsure)

![A screenshot of the Audio section within Timing and Control Points popup menu](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b595b_audio_section.png)

Vous pouvez maintenant utilisez jusqu'a 2 échantillon customisé! Pensez aux possibilités!

Vous pouvez savoir dans le .osu quelle échantillon a été appliquer a une section de timing en cherchant le 5ème flag

`500,-100,4,2,1,75,0`

- Le ˋ1ˋ dans la 5ème section ici indique sue cette section utilise l'échantillon customisé 1. C'est cette version du jeu qui vous laisse utilisé jusqu'a 2, si le nombre est plus haut, le je le lira comme si il n'y a aucun remplacement, donc pas de triche! osu! n'en remplacera aucun en sauvegardant au moins.

## b699 support pour des maps en modes specific

Maintenant quand vous téleversez une map, le gamemode devrait être correctement identifier. Je ne peux pas tester cela vu que le BSS de titanic n'est pas encore prêt, mais cela veut dire que les maps de ce client devrait apparaitre proprement en tant que maps taiko, pas juste des maps taiko qui était forcé d'être jouable en standard aussi lol. CtB n'est pas encore supporté

## b699 temps de kiai

Le temp de Kiai peut maintenant être ajouter! Ceci rajoute quelque effets visuels au jeu pendant les section de timing qui l'utilise. Pour quelque raisons ceci a des modifications de gameplay aussi, telle que faire en sorte que certains objets donne plus de points en taiko, changer la distance de disparrission de HD pour qu'elle soit plus basse. De plus, il y a un effet de lueur sous les notes, en en CtB l'effet de lueur est là ou le fruit va tomber.


## b699 Faire pivoter...

![Rotate by... popup as seen in b699](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b699_rotate_by.png)

Vous pouvez finalement pivotez par montants arbitraire, soyez ravi! Un truc embettant est que vous devez ecrire un montant dans cette version, donc ce n'est pas le monde des Bisounours, et aucun aperçue, ecrivez un nombre, appuyez sur OK et regardez l'horreur que vous avez déchainner j'imagine mdr.

## b753a 'grid snap' et 'beat snap divisors' sauvegardez dans le .osu

Changement de qualité de vie, ces choses sont maintenant sauvegardezs dans le .osu, donc vous pouvez voir quelles paramètre le 'beatmapper', plutôt que vos derniers que vous avez utilisez.

# b1077a à b1218 (v6)

.osu v6 fixed an issue with stacking objects over spinners and animation speeds in storyboards that existed in .osu v5's. Bugs like this are maintained for compatibility in gameplay, but are not visible in the editor. The editor updates the map to the most recent format when you open it (this is why you get prompted to update old maps if you simply just open them and do nothing, and then exit)
Le .osu v6 a réparé un probleme avec l'empilement d'objet	au dessus des spinners, et la vitesse d'animation dans les storyboards qui existaient ans les .osu v5. Les bugs comme ça sont maintenu pour la compabilité dans le jeu, mais ne sont pas visible dans l'éditeur, L'éditeur met à jour la 'beatmap' au format le plus recent quand vous l'ouvrez (c'est pourquoi vous êtes demandez de mettre à jour les vielles 'beatmaps' si vous les ouvrez simplement et faite rien, et puis quittez) (unsure)

# b1533 (v7)

Ceci est la seul version que nous avons qui crées des .osu v7. Ceci répare un une erreur de calculation avec les 'slider's bezier. 

# b1652 à b1672 (v8)

Selon les documentations, 3 changements ont été fait avec la v8.

## additions de mm

Des ”tiques de sliders par beat” constant sont maintenant généré.

## Drainage de PV vers les pauses

Je ne sais pas si cela a été rendu plus difficile ou plus facile. Personne se soucie de comment les PV marche exactement, donc ce genre de choses ne sont jamais entièrement documenté.

## triple roulement de tambours en taiko

Ce n'est pass claire si ils ont été rajouté, ou réparé dans cette version.

# b1700 à b20120916 (v9)

## b1700 seulement des 'sliders' bezier

Peppy decided to wage war on all the older slider curve types. .osu v9's contain only bezier sliders. Linear sliders are recreated through red anchors or 2 point beziers, catmulls and linears are no longer selectable using the slider curve type hotkeys. Any slider curves your map has when you open them in these clients will be maintained, but if you try adding any new points to any old slider it becomes a bezier.
Peppy à décidé faire la guerre sur tout les types de vielles courbure de slider. Le .osu v9 contient seulemnt les 'sliders' bezier. Les sliders Linéaire sont recréer à travers les ancres rouges, ou 2 points bezier, Catmull et Linéaire ne sont plus selectionable en utilisant les raccourcis de clavier de type de roubure de slider. N'importe quelle type de slider que votre map à en quand vous l'ouvrez dans ces clients seront maintenu, mais si vous esayez d'ajouter un nouveau point a un vieux 'slider' il deviendra un bezier. (not too sure)

## b1700 nouveau combo de spinner ne sont plus imposé

This is a change that peppy has flip flopped on many times. In modern stable this is actually enforced again, but on modern lazer it isn't. Older versions had it not enforced, then it became enforced.
C'est un changement que peppy a floppé dessus plusieurs fois. Dans la version moderne de stable ceci est actuellement encore imposé, mais sur la version moderne de Lazer, ça ne l'est pas. Dans les vielles versions ça ne l'était pas, mais il est devenu imposé. (unsure)

# b20121003shine.test à b20121203 (v10)

Comparé aux anciennes mis à jour du format .osu, ceci amène plusieurs nouvelles fonctionalités au format!

## b20121003shine.test éditeur mania
![b20121003shine.test mania editor](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b20121003_mania_editor.png)

Ceci est la toute preière version qui supporte mania! Elle a quelque différences comparé à la version moderne. Cette version du jeu utilise une colone de grille très basique avec des 'hitobjects' normaux. Ceci donne une bonne vu de comment les 'beatmaps' mania sont vraiment enregistré dans le fichier .osu. L'air de jeu esr divisé en combien de colone la map as (basé sur la taille des cercles). Les 'sliders' sont utilisé pour les LNs, le bouton mderne ”Hold Note” n'existe pas encore.

Mania était tellement éxperimental durant le temps de ce format que les 'beatmaps' n'était pas autorisée d'être ranké durant cette vesion du .osu sur Bancho. Toute les 'beatmaps' mania qui ont était faite durant cette époque était mise à jour en meme temps que l'éditeur s'améliorait.

## b20121003shine.test additions d'échantillons
![b20121003shine.test SamepleSet Additions](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b20121003_sampleset_additions.png)

Ceci développe grandement le 'hitsounding', vous pouvez ajouter la version 'soft', 'normal', et 'drum' a n'importe quelle hitsound au dessus de l'échantillion d''hitsound' original, créant plus de profondeur.

## b20121003shine.test champs d'artiste et musique romanisé
![b20121003shine.test Song Setup](https://raw.githubusercontent.com/osuTitanic/wiki/refs/heads/main/wiki/Editor_Differences/img/b20121003_song_setup.png)

Vous pouvez finalement utilisez la langue d'origine pour le nom d'artiste et de la musique, et les mettre en Anglais aussi. Ceci est une fonctionalité importante sur Bancho, si le nom de l'artiste est écrie dans une autre langue sur Bancho, vous devez utiliser les 2 champs conformément aux critères de classement. Prenez l'artiste Japonaise monet, son nom est toujours écrie en Anglais, donc seulement le champs normal est utilisé. Ceci n'est pas une règle imposé de titanic en revanche.

## b20121003shine.test BeatmapID et BeatmapsetID enregistré diretement dans le fichier .osu.

Ceci est important, car des outils tel que ”Mapset Verifier” vérifie que ces tags sont là, et donc sont des exigence tacites aux Critères de Classement sur bancho. Cependant titanic ne force pas cela.

## b20121003shine.test répare chaque partie de 'sliders' bezier qui était 1/50 de seconde trop courte

Cec est la vrai raison pour peppy d'avoir incrémenté au format v10. C'est la deuxième fois qu'un .osu ai été incrémenté du au problème avec les 'sliders' Bezier mdr

## b20121003shine.test osz2

Ceci est la toute première version de osu! qui téleverse des 'beatmaps' en osz2. La partie importante de cette fonctionalité est que seulement les cients qui supporte osz2 peuvent actuellement téleverser des 'beatmaps' sur titanic. Donc si vous voulez téleverser vos 'beatmaps', ceci est la première evrsion que vous pouvez utiliser!

# b20121223 (v11)

Ceci est la seul version que nous avons qui crée des .osu v11.

## ”seulement” les 'sliders” à courbure parfaite

Il y a peu de version de osu qui enregistre tout les 'sliders' en courbure parfaite, vous pouvez voir cela dans des 'beatmaps' comme celle ci: https://osu.ppy.sh/beatmapsets/66346#osu/193641 . Ceci est vraiment similaire à ce que les .osu v9 et v10 font avec les 'sliders' bezier.

## sauvegarde des 'sliders' linéaire, à courbure parfaite, bezier dans le fichier .osu

A un moment cela à été changé à la façon que nous connaissons ous aujourd'hui. Honnetemment je ne suis meme pas sure si ceci est un changement de la v12 ou de la v11 pour l'instant.

Les sliders à 2 points sont toujours sauvegardé comme linéaire, 3 points en courbe parfaite, 4 points ou plus comme bezier. Ceci est comment osu! lit les 'beatmaps' qui prétende que tout les 'sliders' sont à courbe parfaite, donc autant les sauvegarder comme cela pour que ce soit plus simple à analyser dans le fichier .osu.

# b20130303 à mi-2014 (v12)

Je n'ai aucune idée de ce qui a été rajouté

# mi-2014 à mi-2015 (v13)

Cette verrison rajoute la possibilité d'ajouté des valeurs décimal de difficulté au 'beatmaps'! Au moment ou cela a été rajouté, vous pouviez seulement faire des incréments de .5, mais cela sera changé plus tard pour supporté des incréments de .1. Mais, notez bien que les paramètres de difficulté décimal sont contre les critère de classement sur titanic! Ne téleverser pas des maps avec AR9.5 par exemple.

# mi-2015 à aujourd'hui (v14)

This versions adds per node sampleset changes to sliders (or juice streams) for Catch the Beat. I'm a CtB and I don't even know what this means, and I have no idea if anyone uses this to be honest.

# Late 2018 to now (v128)

This is the .osu version for all maps made on lazer. Inside lazer you can export maps in compatiblity mode (osz) for editing on stable, or you can save in the lazer format (olz) for editing on lazer. As of the time of me writing this (7-25-2024), there has never been a 100% pure .osu v128 ranked, as all lazer maps ranked on Bancho, or Titanic have been updated on stable during the ranking process, bringing the .osu version back to v14. However, using my modded client you can actually upload the map as a pure .osu v128, so if you are feeling adventurous you could be the very first one to do so!

# b20130303 Digital Client++

This a modded mapping client made by Digitalfear117, with help from Nikku, Tree, and Levi! This offers many legacy and stable features for mappers to use, and a few extra new ones as well.

## slider curve type swapping

Just like older clients, you can press A, S, or D to change slider curve types. Unlike old clients you can also press F to change to perfect curves too! This is the first client that you can easily choose any slider curve type.

## expanded beat snap divisor and distance snap

Using the Unhinged Slider Curve Type, and Unhinged Beat Snap Divisor options in the editor, you can use DS from 0.1x to 16x, and you can map from any beat snap 1/1 to 1/32. These features do also fully work when exported to stable or lazer, so get crazy with it!

## fixed sv decimal rounding

For some reason this version of osu! would round sv's like 0.95 to 1.00. This has been fixed in my client

## decimal difficulty settings

You cannot use AR's such as 9.5 when uploading maps to titanic. They must be whole numbers. However, if you wish to map for stable or lazer, you can enable this in Compose. Using decimal difficulty settings will save the map as a .osu v13 instead of a v12.

## taiko and catch the beat editors

Although modern stable doesn't seem to offer much for Taiko and CtB mapping, they do actually have a few more features. For CtB distance calculation only changes when you move something in the X coordinate, and for Taiko you can actually see the color of the don and kats based on NC's.

## uploading older .osu formats

All other osu clients force update your .osu file to the version they are built around, however my client is different. You can import your map from another client, and go directly to the upload button. It will ask you if you want to force save, and you can hit No. Doing this will skip the saving process, allowing you to upload any map from any client in a pure fashion! Try this for uploading .osu v9's and earlier, and .osu v128's!
