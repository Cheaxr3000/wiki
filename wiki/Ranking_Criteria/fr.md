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

- **Mapsets must have a total drain time of at least 90 seconds (1 minute and 30 seconds).**
- **Difficulty names must have progression.**
  - Easy -> Normal -> Hard -> Insane -> Expert is default.
  - Logical naming schemes like Seed -> Sprout -> Tree are okay too.
  - **Exception:** The hardest difficulty can use a custom name, like Normal -> Hard -> *Melancholy*.
- **Don't skip difficulties.** For example, if you have Normal and Insane difficulties, you need a Hard too.
- **A [guest mapper](https://osu.ppy.sh/wiki/Beatmap/Guest_difficulty) can't create more difficulties than the [host](https://osu.ppy.sh/wiki/Beatmap/Beatmap_host).**

### Slider Usage

- **Using Perfect Curve sliders is highly discouraged.**
  - Perfect Curve sliders are the type of sliders creating when a slider has 3 control points in clients b20121106 or later
  - ![Example of Slider Curve Types](https://github.com/user-attachments/assets/ac50d9f8-ceb2-4fbe-9420-9cd1eba9de60)
  - These sliders get converted to the Catmull curve type on older clients. This causes slider shapes to differ greatly, creating gameplay differences on those clients. To avoid this issue we highly encourage mappers to use any of the other curve types. In the image above you can see how identical slider skeleton lines create completely different slider paths on each curve type.
  - **Exception:** Perfect Curve sliders with extremely small amounts of curve will generally convert fine, but for safety we recommend not using them.
  - For information on how to avoid using Perfect Curve, [check out this forum post](https://osu.titanic.sh/forum/13/t/731/)!

### Visuals

  - **Avoid using combo colours, slider borders or hitcircleoverlays with ~50 luminosity or lower.** Dark colours like these impact readability of approach circles with high background dim and the other elements partially give up their functions as borders.
  - **Avoid using combo colours and custom slider track colours with ~220 luminosity or higher during kiai times.** They create bright pulses which can be unpleasant to the eyes.

### Hitsounds

- **Maps must be [hitsounded](https://osu.ppy.sh/wiki/Beatmapping/Hitsound),** excluding osu!mania maps.
- **Every clickable object must have audible feedback.**

### Timing

- **Maps must be correctly timed.** This includes BPM and time signatures.
- **All difficulties must use the same timing.**
- **Do not change timing to adjust slider velocity.**
- **Objects must be snapped to timeline ticks.**
- **Only one object is allowed per tick,** excluding osu!mania maps.
- **Manual lead in time must be added to ensure the first object starts after 1500ms**

## Metadata

- **Metadata must be accurate.**
  - Use a [primary metadata source](https://osu.ppy.sh/wiki/Beatmap/Primary_metadata_source).
  - If the song has a Ranked or Loved map, use that map's metadata unless it's blatantly wrong.
- **Use [Modified Hepburn romanisation](https://en.wikipedia.org/wiki/Hepburn_romanization#Features) for Japanese words.**

### Tags

- **Add usernames of anyone who contributes to the map.** This doesn't include modders.
- **Add the song's [genre and language](https://osu.ppy.sh/wiki/Beatmap/Genre_and_language).**
- **Add `featured artist` if the song is in the [Featured Artist catalogue](https://osu.ppy.sh/beatmaps/artists).**
- **Other tags must be relevant to the song/map.**

### Title

- **Songs shortened for TV must have `(TV Size)`.**
- **Replace game version markers with `(Game Ver.)`.**
- **Replace short version markers with `(Short Ver.)`.**
- **Use `(Cut Ver.)` to indicate an unofficial song cut.**
- **Use `(Extended Edit)` to indicate an unofficial song extension.**
- **Use `(Sped Up Ver.)` to indicate an unofficial song tempo increase.** For some genres, `(Nightcore Mix)` is an okay alternative.

### Source

- **Use the Source field if the song is from another media source, like a game, movie, or event.**

## Files

- **Don't use inappropriate content.** See [song content rules](https://osu.ppy.sh/wiki/Rules/Song_content_rules) and [visual content considerations](https://osu.ppy.sh/wiki/Rules/Visual_content_considerations).
- **Don't include unused files in the map folder.**

### Song

- **Use `.mp3` or `.ogg` file formats.**
  - At most 192 kbps for `.mp3` files.
  - At most 208 kbps for `.ogg` files.
  - At least 128 kbps for any filetype.
- **One song file must be used for all difficulties.**
- **Set a consistent preview point for all difficulties.**

### Hitsounds

- **Hitsound files must be at least 25 ms long and use `.wav` or `.ogg` file formats.**
  - Do not use `.mp3`.
  - **Exception:** Use [this file](https://up.ppy.sh/files/blank.wav) for silent hitsounds.
- **Hitsounds must not be [delayed](https://osu.ppy.sh/wiki/images/Ranking_criteria/Simplified_ranking_criteria/img/delay.png).**

### Background

- **Every difficulty must have a background adhering to the following:**
  - **Minimum width:** 160 px
  - **Minimum height:** 120 px
  - **Maximum width:** 2560 px
  - **Maximum height:** 1440 px
  - **Maximum file size:** 2.5 MB
- **Link the source of the map's background in the description.**

### Video

- **Videos must adhere to the following:**
  - **Maximum video resolution:** 1280x720
  - **Video encoding:** H.264
- **The audio track must be removed from video files.**

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
