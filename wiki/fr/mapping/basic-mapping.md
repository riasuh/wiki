---
sidebar: auto
prev: ./basic-audio.md
next: ./intermediate-mapping.md
description: Apprenez toutes les informations et les meilleures pratiques dont vous avez besoin pour faire une bonne première map!
---

# Les bases du mapping
_Si vous êtes un nouveau mapper, lisez cette page de haut en bas. Chaque mot. Chaque image. Cette page vous donnera toutes les informations et les meilleures pratiques dont vous avez besoin pour faire une bonne première map!_

* [Lexique](./glossary.md)

## Prêt à mapper?
**Avez vous...**

1. [x] [Téléchargé Audacity](https://www.audacityteam.org/) et choisi un [éditeur de map](/fr/mapping/#ressource-pour-l-edition-de-map)?
2. [x] Configuré [votre fichier audio](/fr/mapping/basic-audio.md) pour confirmer votre bpm et vérifier que vous avez une bonne intro/outro ?
3. [x] [Exporté](./basic-audio.md#exporting) votre fichier audio en format OGG ?

::: tip Toutes ces choses ont-elles été faites ? SUPER! Vous êtes maintenant prêt à vous plonger dans votre éditeur préféré et à commencer à mapper! Dans le cas contraire, cliquez sur les liens de la liste des tâches pour plus d'informations. :::

## Les fondamentaux
Avant même de penser à mapper, vous devez comprendre les bases.

### Fichiers de Map
Quel que soit l'éditeur avec lequel vous choisissez de mapper, chaque map a besoin de :

* **Fichier audio:** Format OGG, vous devez avoir ceci prêt avant de pouvoir mapper. Nommez-le `song.ogg`
* **Image de couverture:** JPG ou PNG, l'image doit être parfaitement carrée et 512 pixels par côté est recommandé. Vous devez avoir ceci avant de pouvoir publier votre map.  Nommez-la `cover.jpg` ou `cover.png`
* **Fichier d'info:** Contient toutes les métadonnées de votre carte dans son ensemble. Les choses dans ce fichier s'appliquent à TOUTES les difficultés (i.e., nom de la chanson, nom de l'artiste, nom du mappeur, nom du fichier de la chanson, nom de l'image de couverture, difficulté, vitesse d'arrivée de la note, etc.). Ce fichier est automatiquement créé par votre éditeur.
* **Fichiers de difficulté:** Un par difficulté dans votre map. Les choses dans ce fichier s'appliquent à une seule difficulté (c.-à-d. le placement de notes, le placement de lumière, etc.). Ces fichiers sont automatiquement créés par votre éditeur.

Certains éditeurs créeront automatiquement un dossier `autosaves` (sauvegardes automatiques) où vous pourrez récupérer des copies plus anciennes de votre travail si nécessaire. Lorsque vous êtes prêt à publier votre musique , vous devez avoir au moins 4 fichiers.

::: warning Les caractères spéciaux dans les langues telles que le japonais (日本語/にほんご), le Kaomoji (٩(◕‿◕｡)۶), le chinois (汉语/漢語), l'arabe (اَلْعَرَبِيَّةُ‎) et les accents (Ä/é/ó) ne sont pas entièrement pris en charge par BeatSaver. Utiliser ces caractères dans les métadonnées ou dans les signets de la map peut causer des problèmes. :::

### Types de bloc
<!-- markdownlint-disable MD013 -->
|                    Directional Blocks                     |                   Blocs point                   |                                  Bombes                                  |                                 Murs                                 |
|:---------------------------------------------------------:|:-----------------------------------------------:|:------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
|  ![Directional Block](~@images/mapping/arrow-block.png)   | ![Blocs point](~@images/mapping/dot-block.png)  |                   ![Bombe](~@images/mapping/bomb.png)                    |                  ![Mur](~@images/mapping/wall.png)                   |
| Doit être coupé dans<br />la direction de la flèche | Peut être coupé dans n'importe quelle direction | Inflige des dégâts lorsque coupé <br />mais est sûr pour le joueur | Inflige des dégâts au joueur mais<br />est sûr pour les sabres |
<!-- markdownlint-enable MD013 -->

**Quelques précisions sur les murs:**

* Les murs standard peuvent être reconnus par n'importe quel casque VR et ont la plus grande compatibilité. Les nouveaux mappers devraient s’en tenir à ces derniers jusqu’à ce qu’ils soient un peu plus expérimentés.
* There are a few types of "hack" walls that do not require the Mapping Extensions mod: fast walls (fly by you fast), hyper walls (fly by you SUPER fast), and fake walls (look like normal walls but don’t cause damage).
* Bien que ces types de murs soient pris en charge dans certains éditeurs, ils abusent des mécanismes du jeu de base et sont considérés comme inclassables.
* Read up more on base game walls in [Intermediate Mapping](./intermediate-mapping.md) and "fancy" mapping/noodle extensions walls in [Extended Mapping](./extended-mapping.md)

**Quelques précisions sur les bombes:**

* Les boîtes de collision des bombes sont plus petites que les boîtes de collision de blocs, elles sont même plus petites que le modèle de la bombe.
* Les bombes sont difficiles à voir quand l'éclairage n'est pas activé. Vérifiez que votre map n'est pas trop sombre lorsque les bombes arrivent. Consultez [Les bases du lighting](./basic-lighting.md) pour plus de conseils.
* Les bombes peuvent toujours être coupées après avoir passé le joueur.

### Répartition des blocs
Cela varie en fonction de la difficulté ciblé et du public pour lequel vous êtes en train de mapper. Par exemple, certains joueurs dans les difficultés inférieures peuvent être submergés par une répartition équilibrée entre les trois rangées par rapport à un joueur plus expérimenté qui peut gérer plusieurs blocs sur les rangées et colonnes. La distribution de blocs peut également varier entre les styles de mapping à un même niveau de difficulté.

Pour plus d'informations sur l'utilisation de blocs dans les lignes/colonnes dans différentes difficultés, voir [Mesure de la difficulté](#gauging-difficulty-down-mapping).

::: tip Si vous utilisez [Mediocre Map Assistant 2](./mediocre-map-assistant.md) comme éditeur vous pouvez appuyer sur <kbd>SHIFT</kbd>+<kbd>TAB</kbd> pour ouvrir le vérificateur d'erreur, puis cliquez sur le bouton <kbd>panneau de statistiques</kbd> pour voir cette panneau. :::

## Timing & Rhythme
Avant de commencer à mapper sérieusement, vous devez penser au rythme de la chanson que vous voulez mapper. Vous placerez des blocs sur un ou plusieurs des principaux instruments de la chanson : le battement du tambour, l’instrument principal, la basse, les synthés ou même le chant.

Pour placer des blocs dans le temps avec le rythme, vous devrez changer la précision de votre curseur. La plupart des chansons (mais pas toutes) utilisent la précision du curseur 1/1, 1/2 ou 1/4 pour être dans le rythme. Certaines musiques peuvent utiliser la précision « triplets » ou 1/3 qui peut être difficile à distinguer de 1/4 pour une oreille inexpérimentée. Vous ne devriez pas avoir besoin d'utiliser moins de 1/4 de précision pour la plupart des musiques *y compris* pour mapper le chant.

::: warning  
90 % du temps, le mapping avec une haute précision (1/8, 1/16, 1/32 ou 1/64) rendra votre chanson décalée. Si vous avez besoin d'une grande précision pour que vos notes soient en rythme, alors vous avez un problème avec la configuration de votre fichier audio. Arrêtez et révisez [Configuration audio de base](./basic-audio.md) pour vous assurer que vous êtes en accord avec la musique! :::

|                        Précision du curseur 1/1                        |                        Précision du curseur 1/2                        |                        Précision du curseur 1/3                        |                        Précision du curseur 1/4                        |
|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| ![1/1 Cursor precision screenshot](~@images/mapping/1-1_precision.png) | ![1/2 Cursor precision screenshot](~@images/mapping/1-2_precision.png) | ![1/3 Cursor precision screenshot](~@images/mapping/1-3_precision.jpg) | ![1/4 Cursor precision screenshot](~@images/mapping/1-4_precision.png) |
|                          1 bloc par battement                          |                          2 bloc par battement                          |                          3 bloc par battement                          |                          4 bloc par battement                          |

Quand vous faites le timing d'une map, il est important de vérifier au DEBUT que la musique est bien en rythme avec la piste de l'éditeur. Si votre musique n'est pas alignée, revisitez la page [Mise en place de l'audio basique](./basic-audio.md) du wiki pour des conseils.

::: danger ATTENTION  
Si votre musique n'est pas alignée, cela rendra **très** difficile de placer des blocs en rythme avec la musique. Faites les choses comme il faut avant de commencer ou vous risqueriez de devoir tout remapper plus tard! :::

|                                 Audio non aligné                                 |                             Audio correctement synchronisé                              |
|:--------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|
| ![Editor view with audio not properly synced](~@images/mapping/audio-broken.png) | ![Editor view with audio synced to the editor track](~@images/mapping/audio-synced.png) |
|                Needs audio edits, start offset, or has wrong bpm                 |                                Vous êtes prêt à mapper!                                 |

### Les notes timing
Consider starting the mapping process with placeholder or "timing" notes. Dropping a "dot note" placeholder can help you figure out whether or not your map is on time and where you should consider using extra emphasis **before** you invest a ton of time creating patterns. Listen to make sure the editor hit sounds are in time with the beat.

::: tip  
Tout le monde n'utilise pas de notes timing, mais en tant que nouveau mappeur elles peuvent être un moyen utile de s'assurer que vos map sont bien en rythme. :::

### Overmapping & Undermapping
Placez délibérément des blocs qui correspondent à la musique. Ne placez pas plus de blocs que nécessaire pour rendre la map difficile. Certaines chansons n’ont jamais été conçues pour être des map très denses Expert+ et c'est normal.

* **Overmapping** is the (bad) practice of placing more blocks than there are sounds. Ne le faites pas.
* **Undermapping** is the very acceptable practice of skipping some notes/beats (especially at lower difficulties).

### Emphasis & Consistency
We’ll go into more detail on this in [Intermediate Mapping](./intermediate-mapping.md) but, as a new mapper you should understand at least the basic ideas of emphasis and consistency and how they impact your map.

**Emphasis** is how much "weight" you give each hit.

* Consider the base sound your mapping to to be a single hit (one block), including quiet or chill sections
* When the sound is "bigger" or you have two different instruments hitting on the same beat you can think about using a double hit or a stack (two blocks).
* For only the biggest sounds in the song you could use a double tower (four blocks, two for each hand) or other heavyweight pattern, but many songs never need this amount of emphasis.

Many new mappers instinctively want to use double hits all the time, but remember that those are heavy emphasis and if *every sound* is emphasized then *nothing* feels like it has extra weight.

Another way to think about it is that you want the energy and effort of the hit to match the energy and power of the sound. Nobody screams at the top of their lungs on every vocal, or in every instrument note. You want the powerful notes, the powerful vocals, to stand out from the rest of the song. Even if most of the song might sound loud or (you think) emphasized, there's always notes that sound above them. Be it through volume, or through energy. So when mapping, see what is your baseline energy, map that as singles. Anything above that, then do towers/doubles/windows/jumps, whatever best matches that energy.

**Consistency** is mapping the same sound with the same weight when it appears.  
Mapping consistently does NOT always mean to copy/paste/mirror, though there are some times when that is appropriate. If you choose to map a particular big sound as a double, for example, that same sound should always be mapped with a double.

## Meilleures pratiques pour les pattern
Cette section détaille les principes à suivre pour avoir une map jouable et agréable.

**Cyrix** a créé une vidéo récapitulative en anglais, [pattern à éviter en tant que nouveau mappeur](https://www.youtube.com/watch?v=mgGaqZ20Scw), des problèmes les plus courants qui sont couverts dans cette section.

### Blocs de vision
Les blocs de vision sont des pattern qui bloquent la vision du joueur et rendent difficile la lecture d'une map, ce qui peut la rendre inconfortable à comprendre. La cause principale des blocs de vision est l'utilisation des deux positions du milieu de la piste, mais il y a un risque de blocage de vision à chaque fois que la rangée du milieu est utilisée.

**Les blocs de vision peuvent être évités:**

* En n'utilisant pas les deux positions centrales de la piste.
* En s'assurant que les blocs qui suivent n'importe quoi dans la rangée du milieu sont: soit assez éloignés, soit dans une autre position à droite ou à gauche du bloc.
* En s'assurant que le joueur est poussé sur le côté grâce des obstacles ou des pattern afin que les positions au centre ne bloquent plus complètement le joueur.

<!-- markdownlint-disable MD013 -->
|                           Placement de bloc idéal                            |                     Placement de bloc de vision                     |
|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------:|
|          ![No Vision Blocks](~@images/mapping/no-vision-blocks.jpg)          |           ![Face Notes](~@images/mapping/face-notes.jpg)            |
| When you’re getting started, stick<br />to the perimeter of the track. | These are called face notes.<br />Avoid them as a new mapper. |
<!-- markdownlint-enable MD013 -->

::: tip  
**Mediocre Map Assistant 2** a un vérificateur d'erreur pratique intégré qui peut trouver des blocs de vision. En savoir plus dans le [Guide d'utilisateur MMA2](./mediocre-map-assistant. md#error-checker). :::

### Doubles Directions & Resets
Les doubles directions (ou DD) sont ce que vous obtenez quand vous avez deux blocs de la même couleur dans la même direction en un très court laps de temps. Diagonals, or any change of only 45 degrees between blocks, are considered to be DDs with both the cardinal directions they combine.

::: align center ![Blue up right diagonal block](~@images/mapping/bnur.png)is a DD with both ![Blue up block](~@images/mapping/bnu.png) and ![Blue diagonal block](~@images/mapping/bnr.png) :::

Les doubles directions obligent le joueur à doubler sa vitesse de swing par rapport à un pattern « standard » de haut en bas. Les joueurs doivent faire un mouvement vers le bas, puis ramener la main vers le haut et enfin vers le bas encore, ce qui fait beaucoup de mouvement inutiles. Alternez la direction de chaque autre bloc pour une meilleure fluidité.

De nombreux nouveaux mappers utilisent des doubles directions pour simuler la sensation de tambour. While this *feels* like it makes sense, drums have rebound when you hit them and imaginary computer blocks... don’t. Le jeu s'appelle Beat Saber, pas Beat batteur!

|                           Fluidité standard                           |                            Doubles Directions                             |
|:---------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| ![Image of standard up down flow](~@images/mapping/standard-flow.jpg) | ![Image of double directionals](~@images/mapping/double-directionals.jpg) |
|                   Une bonne pratique de mapping :)                    |                          Non! Ne faites pas ça !                          |

Les **resets **de DD peuvent être* utilisés* (généralement dans des cartes plus “dansées”) si vous donnez au joueur suffisamment de temps pour réinitialiser ses mains à une position neutre. Cela signifie généralement qu’il n’y a pas de DD à moins de 2 battements pour les chansons avec un bpm « normal » et bien plus de 2 battements pour les chansons avec un bpm élevées.

::: warning  
Si vous utilisez intentionnelement des DD dans une map "dansée", vous devrez rendre votre NJS plus lente et le spawn offset plus long pour donner au joueur suffisamment de temps pour réagir. :::

::: danger Wrist resets are when you change the forehand/backhand flow of a a pattern mid-stream causing your player to roll their wrist to reset flow. They can break normal human body mechanics and put players at serious risk of joint damage. Do not use wrist resets at high precision! :::

When long periods of time pass between notes, the player will reset their arm position so it’s often preferable to start the new section with a down block.  In gray areas of time, like 3 seconds without notes, it is up to the mapper to reset the player or to continue the flow.

Want to learn more about resets? Read [Intermediate Mapping](./intermediate-mapping.md)!

### DO: Mapping with Flow
Outside of easy and normal difficulties, mapping with flow is an absolute must. Human bodies are incredible machines but there are certain ways that joints are meant to move and using patterns that violate those mechanics is a recipe for injuring your player.

Parity is the concept that each block direction is played with either a backhand swing or a forehand swing. The black line in the diagram below illustrates this forehand (below the line)/backhand (above the line) divider for the left and right sides.

::: align center ![Parity diagram showing the forehand/backhand line for each block color](~@images/mapping/parity_diagram.jpg) :::

When mapping with flow you are striving to always cross this parity line with the most natural movement possible. Effectively, your player should always be alternating between forehand and backhand every swing.

This video demonstrates the basics of parity: [YouTube](https://youtu.be/tLQK4gN3bDc)

A thing important to keep in mind, especially if you are new to the game or mapping, is that the concept of parity is most obvious for wrist players. If you do not play with your palm directly facing the ground, then you might struggle to understand why some parity breaks are uncomfortable. Remember that while it may feel fine to you, players have different grips and styles. Proper parity feels good for everyone, not just some playstyles.

::: tip  
When proper flow is achieved the player should be physically capable of getting full points on each block, even if they don’t have the skill or interest in doing so. See the [Scoring](/grips-and-tricks.md#scoring) section of the wiki for more info. :::

|                              Angle 0°                              |                              Angle 45°                               |                              Angle 90°                               |                               Angle 135°                               |                               Angle 180°                               |
|:------------------------------------------------------------------:|:--------------------------------------------------------------------:|:--------------------------------------------------------------------:|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| ![0 degree angle change between blocks](~@images/mapping/0deg.png) | ![45 degree angle change between blocks](~@images/mapping/45deg.png) | ![90 degree angle change between blocks](~@images/mapping/90deg.png) | ![135 degree angle change between blocks](~@images/mapping/135deg.png) | ![180 degree angle change between blocks](~@images/mapping/180deg.png) |
|                             Non. (DD)                              |                              Non. (DD)                               |                                Maybe.                                |                                  Oui.                                  |                                  Oui.                                  |

**Basic Flow Concepts:**

* The higher your note precision, the more you want to stick to 180° (up/down) and 135° (up/down/diagonal) patterns.
* 90° transitions that cross the parity line should only be considered with enough time to play smoothy.
* Make sure that you have the right setup (the pattern immediately before) and escape (the pattern immediately after) for a comfortable swing at whatever speed you’re mapping.
* Be conscious of your timing, you can get away with more at sub-160 BPM tempos with lower note precision than you can in high BPM songs. Map for the style of song you’ve selected.

### DON’T: Forbidden Patterns
These are called forbidden patterns for a reason. There is no reason in the world to use these because they're dangerous to either the player's hardware, the player's joints, or they go against the scoring system. You may have played maps that included these but that doesn't make them ok.

#### Handclaps
|                             Illustration                             |                               Editor View                               | Explication                                                                                                                                                                                                                                                                                                                                                                                  |
|:--------------------------------------------------------------------:|:-----------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a handclap](~@images/mapping/controller-smash.png) | ![Editor view of a handclap](~@images/mapping/controller-smash-alt.png) | Pointing blocks at each other may cause the player to smash their controllers together when playing for max points. Don’t do it, no exceptions.<br /><br />Note: Different VR sets have different controllers. Vive wands are much bigger than Oculus touch controllers and Index knuckles... don’t put your players’ hardware at risk! *AKA Controller clash, Controller smash* |

#### Hammer Hits
|                           Illustration                           |                             Editor View                             | Explication                                                                                                                                   |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a hammer hit](~@images/mapping/hammer-hit.png) | ![Editor view of a hammer hit](~@images/mapping/hammer-hit-alt.png) | Any directional block pointing towards a bomb on the same plane is just evil (and undermines the scoring system). Don’t do it. No exceptions. |

#### Disembodied notes
|                                 Illustration                                 |                                   Vue éditeur                                   | Explication                                                                                                                                                                                                                          |
|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of disembodied notes](~@images/mapping/disembodied-notes.png) | ![Editor view of disembodied notes](~@images/mapping/disembodied-notes-alt.png) | Do not hide blocks on the other side (or inside) of walls. Most of the time, these are simple mistakes that people don’t find because they don’t adequately playtest their maps (NOTE: Always [playtest](./#playtesting) your maps!) |

#### Rapid Wall Dodge
|                                Illustration                                |                                  Vue éditeur                                  | Explication                                                                                                                                                                                                                                                                                                                       |
|:--------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of rapid wall dodge](~@images/mapping/rapid-wall-dodge.png) | ![Editor view of rapid wall dodge](~@images/mapping/rapid-wall-dodge-alt.png) | Keep head movement slow and predictable. Do not force the player to very quickly move from one side of their play space to the other. Wall dodges are fine (and fun!) to use but allow *at least* 1.5 beats for the player to switch sides for higher BPM songs. You don’t want to risk them bumping into things or falling over. |

#### Danger Dash
|                           Illustration                           |                             Vue éditeur                             | Explication                                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of danger dash](~@images/mapping/danger-dash.png) | ![Editor view of danger dash](~@images/mapping/danger-dash-alt.png) | Never force the player into the far edge of their playspace with 3-width walls or a 2-width wall in the middle. Walls that encompass the two middle columns gives the player very little room to play, and you don’t know how large their play area is or how far they will dash in response to these walls. |

#### Bomb Spam
|                         Illustration                         |                           Vue éditeur                           | Explication                                                                                                                                                                                                                                                                               |
|:------------------------------------------------------------:|:---------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of bomb spam](~@images/mapping/bomb-spam.png) | ![Editor view of bomb spam](~@images/mapping/bomb-spam-alt.png) | Bombs are good for forcing precision, or for punctuating silence, but overuse of bombs should be avoided. Also note that most people hate bombs in general, so they should be used sparingly.<br /><br />**Note:** Precision bombs shouldn't be used more than once per beat. |

#### Cross
|                     Illustration                     |                       Vue éditeur                       | Explication                                                                                                                                                                                                                                                                                                |
|:----------------------------------------------------:|:-------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of cross](~@images/mapping/cross.png) | ![Editor view of cross](~@images/mapping/cross-alt.png) | This large, awkward pattern is difficult to read and can lead to smashed controllers, tangled arms, and ugly vision blocks. Players will likely not read it correctly the first time they see it, but even if they do, it’s not a satisfying motion anyway. Consider using a different pattern altogether. |

#### Hidden Blocks
|                             Illustration                              |                               Vue éditeur                                | Explication                                                                                                                                                                                                                                                                         |
|:---------------------------------------------------------------------:|:------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of hidden blocks](~@images/mapping/stacked-hidden.png) | ![Editor view of hidden blocks](~@images/mapping/stacked-hidden-alt.png) | Blocks should never be stacked on top of one another or in walls. Any combination of blocks are technically stackable in the editor (including bombs and walls). Sometimes these are hard to spot if two identical blocks are stacked. Use the error checker in MMA2 to find these! |

#### Hitbox Abuse
|                              Illustration                               |                                     Vue éditeur                                      | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|:-----------------------------------------------------------------------:|:------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of some hitbox abuse](~@images/mapping/hitbox-abuse.png) | ![Alternate llustration of some hitbox abuse](~@images/mapping/hitbox-abuse-alt.png) | Leave room for the player to swing at each block. In the patterns depicted here, there is not enough room for the saber to slice each block without hitting the other. These are technically still possible to hit, but only by coming in at an angle, and if you have to come in at an angle, you may as well change the block direction to a diagonal anyway.<br /><br />The illustration below from Split, one of the game developers, shows the size of the block hitbox. The **large** outer box is for good hits and the small inner box is for bad hits.<br />![Illustration of block collider hitboxes](~@images/mapping/hitbox-from-split.jpg) |

#### Wide Precision
|                              Illustration                              |                                Vue éditeur                                | Explication                                                                                                                                                   |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of wide precision](~@images/mapping/wide-precision.png) | ![Editor view of wide precision](~@images/mapping/wide-precision-alt.png) | These bombs are incredibly hard to avoid for players with short arms. When the player swings through these blocks, their arms come inward, and hit the bombs. |

### MAYBE: Highly Situational Patterns
These patterns are OK to use but only in very specific circumstances or with very specific setup. It’s best to steer clear of these until you’re much more comfortable with mapping.

#### Flicks
|                      Illustration                      |                        Vue éditeur                        | Explication                                                                                                                                                                                                                                                                                                                                                                      |
|:------------------------------------------------------:|:---------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a flick](~@images/mapping/flick.png) | ![Editor view of a flick](~@images/mapping/flick-alt.png) | "Flicks" of two or more blocks of the same color at 1/4 precision are a difficulty spike, regardless of song tempo. It is the precision here that is important, not the patterns since these examples follow proper flow techniques. Even though flicks are more easily playable in lower tempo songs, they are incredibly difficult to use appropriately and should be avoided. |

#### Triangle
|                         Illustration                         |                           Vue éditeur                           | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|:------------------------------------------------------------:|:---------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a triangle](~@images/mapping/triangle.png) | ![Editor view of a triangle](~@images/mapping/triangle-alt.png) | Triangles are patterns that cause incredibly uncomfortable wrist resets  when used at high precision and speed. The pattern breaks the forehand/backhand mechanic and can injure your player. See the [Mapping with Flow](#do-mapping-with-flow) to revisit this explanation.<br /><br />**Note 1:** Not all triangle shaped patterns are cursed triangles. Make sure you are always crossing the parity line with each swing.<br /><br />**Note 2:** This sort of pattern plays differently at hard difficulties and below when there are a couple of beats between each swing but stay away at Expert and ExpertPlus. |

#### Incorrect Side Hits
|                                     Illustration                                     |                                       Editor View                                       | Explanation                                                                                                                                                                                                                                                                                                                               |
|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of upside down side hits](~@images/mapping/upside-down-side-hits.png) | ![Editor view of upside down side hits](~@images/mapping/upside-down-side-hits-alt.png) | Generally speaking, when making a double crossover, you should put RED on top when slicing left, and put BLUE on top when slicing right. This is a best practice because you don’t have to move your opposite hand as far. The exception is Expert/ExpertPlus, but  **only** if the flow of patterns leads to these placements naturally. |

#### Rapid Crossovers
|                               Illustration                                |                                 Vue éditeur                                  | Explication                                                                                                                                                                                                                                                                                                                                            |
|:-------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of rapid crossovers](~@images/mapping/rapid-crossover.png) | ![Editor view of rapid crossovers](~@images/mapping/rapid-crossover-alt.png) | Give the player time to prepare, and don’t make them cross sides too fast or too often. This pattern takes time to process and it’s a larger motion in-game than it looks in the editor. Also, never put this pattern in the top row. It's also recommended to offset the hits and put one of the two notes on the bottom row to reduce handclap risk. |

#### Wide Inward Doubles
|                                Illustration                                 |                                     Editor View                                     | Explication                                                                                                                                                                                                                                                                                                           |
|:---------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of inward doubles](~@images/mapping/wide-inward-doubles.png) | ![Editor view of wide inward doubles](~@images/mapping/wide-inward-doubles-alt.png) | Inward facing double blocks on the edges or downward facing blocks on the top row are very difficult to hit for small/short players, and uncomfortable for the rest. This should generally be avoided. The exception is Expert/ExpertPlus, but  **only** if the flow of patterns leads to these placements naturally. |

#### Excessive Towers
|                                Illustration                                |                                  Editor View                                  | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|:--------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of excessive towers](~@images/mapping/excessive-towers.png) | ![Editor view of excessive towers](~@images/mapping/excessive-towers-alt.png) | Placing 3 blocks of the same color, vertically or horizontally, may seem fun, but you can achieve the same "hard hitting" effect with just 2. 3 feels excessive in-game. Even when using 2, don’t place anything directly behind them, since visibility will be low.<br /><br />At Expert/+ if you are going to use this for major emphasis, each block needs to be staggered after each other at 1/16 (<200 bpm) or 1>200 bpm) precision, turning this into what is known as a slider. |

#### Awkward Curves
|                                     Illustration                                     |                                       Editor View                                       | Explication                                                                                                                                                                                                                                                                                                                                                                  |
|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of awkward curved swings](~@images/mapping/awkward-curved-swings.png) | ![Editor view of awkward curved swings](~@images/mapping/awkward-curved-swings-alt.png) | Do not place two or more blocks of the same color together that do not face the same way. It is harder to read, feels awkward, and undermines the scoring system. Often, these patterns are used as a way to introduce flair to a map, but it’s really just a crutch for unimaginative mapping. Instead, add flair by introducing original patterns that flow well together. |

#### Detached Walls
|                              Illustration                              |                                Editor View                                | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of detached walls](~@images/mapping/detached-walls.png) | ![Editor view of detached walls](~@images/mapping/detached-walls-alt.png) | Combine your adjacent/ touching walls for a cleaner, less visually cluttered experience. Click and drag (left to right) to create walls wider than 1 column. Scroll to create walls shorter/longer than one beat (or whatever your cursor precision is set to) and click again to finish placing your wall. Don’t ever cover the entire grid with walls as depicted in the illustration. <br /><br />**Note:** This rule goes out the window when you get into wall mapping with Mapping Extensions, though this is NOT recommended for new mappers. |

#### Extended Crouch
|                               Illustration                               |                                 Editor View                                 | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|:------------------------------------------------------------------------:|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of extended crouch](~@images/mapping/extended-crouch.png) | ![Editor view of extended crouch](~@images/mapping/extended-crouch-alt.png) | Consider your target audience when using extended sections of top walls. You can't predict all players' physical ability, so use this in moderation. If you have notes immediately following a crouching section, make the starting direction UP, and consider visibility due to the player’s lower position.<br /><br />**Note:** Avoid placing blocks under a crouch wall, but if you must, always place them on the bottom row sides with horizontal slice directions (or dots). |

#### Corner Crouch
|                             Illustration                             |                               Editor View                               | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|:--------------------------------------------------------------------:|:-----------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of corner crouch](~@images/mapping/corner-crouch.png) | ![Editor view of corner crouch](~@images/mapping/corner-crouch-alt.png) | Consider your target audience when forcing the player to crouch in one corner. As stated above, crouching sections should be kept short because you can't predict all players' physical ability. Forcing the player to additionally move left/right while crouching increases the threshold of full-body range of motion. While this tactic may be fun for some, you don't want to ostracize the players that are incapable of this motion. |

#### Sky Streams
|                           Illustration                           |                             Editor View                             | Explication                                                                                                                                                                                                                                                |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of sky streams](~@images/mapping/sky-streams.png) | ![Editor view of sky streams](~@images/mapping/sky-streams-alt.png) | Avoid repetitive use of blocks in the top row. This causes shoulder strain in addition to top row down notes being annoying to score well on.<br /><br />**Note:** Blocks on the top row in Easy and Normal should be dots and used sparingly. |

#### Visual Clutter
|                              Illustration                              |                                Editor View                                | Explication                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of visual clutter](~@images/mapping/visual-clutter.png) | ![Editor view of visual clutter](~@images/mapping/visual-clutter-alt.png) | Avoid unnecessary visual clutter. Having a directional block point towards/away from a dot block does not serve any functional purpose, and it’s hard to read at a glance. If you’re telling the player to slice in a particular direction, be consistent and make both blocks directional to increase readability.<br /><br />**Note:** At Expert/+ when making sliders it is common to start with an arrow then use dots afterward. |

#### Easy to Miss Patterns
|                                    Illustration                                    |                                      Vue éditeur                                      | Explication                                                                                                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of overlapping hitboxes](~@images/mapping/overlapping-hitboxes.png) | ![Editor view of overlapping hitboxes](~@images/mapping/overlapping-hitboxes-alt.png) | Generally, try to avoid patterns with overlapping hitboxes, as this makes the pattern difficult to hit consistently. The hitboxes are larger than the note, and most players rarely hit the actual note when they swing, making it easy to hit the smaller hitbox within notes that detects bad hits on patterns like this. See [Hitbox Abuse](#hitbox-abuse) for more info. |

#### Arm Tangles
|                          Illustration                           |                            Editor View                             | Explication                                                                                                                                                                                                                                                                                                                                                               |
|:---------------------------------------------------------------:|:------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of arm tangles](~@images/mapping/arm-tangle.png) | ![Editor view of arm tangles](~@images/mapping/arm-tangle-alt.png) | Crossing hands is usually fine, but crossing hands and going in opposite directions vertically causes the player’s arms to hit each other. Reverse these colors and you’re good to go. This is only one example of an arm tangle. Always be aware of where you're leaving your player's arms and how they are going to escape from that position to hit the next pattern. |

#### Face Punchers
|                              Editor View                               | Exaplanation                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Editor view of a face puncher](~@images/mapping/facepuncher-alt.png) | Face punchers are blocks placed in the opposite top corners pointing outwards. This placement requires the player to perform a large crossover in a direction that potentially causes their controllers to smash into their headset. <br></br> **Never** use a double of face punchers. |

## Gauging Difficulty & Down-Mapping

Many mappers tend to map the difficulty level at which they typically play, but there are plenty of benefits to mapping lower difficulties:

* Full spreads can be played and enjoyed by a wider audience.
* They look professional when cruising for new maps, just like the base game maps.
* Players who are good at the game can use your lower difficulties for training, such as accuracy players.

The difficulty of a map is comprised of a combination of *density* (rhythm choice), *complexity* (pattern choice), and *readability* (NJS and Offset). There should be a smooth progression as you work your way down from Expert+ to Easy. When building lower difficulties, it’s important to understand what skills players at different levels have and try to preserve the map's identity as you work your way down the spread.

For more information on mapping lower difficulties than what is on this page, check out [Downmapping](./downmapping.md).

### Pattern Complexity

Maps should always have a progression of complexity from Easy through Expert+. The difficulty of a map is typically rooted in its complexity, with a great deal of attention given to what a player would typically expect at a respective difficulty level.

:::tip Remember You are teaching players different patterns and sight-reading skills with your maps. Make sure you give them time to react before you throw something new at them at each level of difficulty. :::

<!-- markdownlint-disable MD013 -->
| Difficulty | Pattern Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|:----------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  Expert+   | &#8227; Welcome to the wild west! You can throw any good mapping practices at your player here.<br />&#8227; Parity is expected at this level, especially for high BPM songs. Lower BPM songs may be more lenient but parity breaks are discouraged.<br />&#8227; Always be mindful of common errors, such as resets and vision blocks.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|   Expert   | &#8227; All note directions are viable here in any proportion.<br />&#8227; All note positions viable here in any proportion. For patterns of wider spacing, give them enough reaction time and be mindful of the player’s stamina.<br />&#8227; Any color, any lane is fine. Crossovers should be used wisely and not combined with other weird patterns.<br />&#8227; Flow is critical. Parity will make or break your map.<br />&#8227; All emphasis options are on the table, including stacks and sliders.<br />&#8227; All obstacles are fair game, but be wary about creating vision blocks.                                                                                                                                                                                                                                                         |
|    Hard    | &#8227; All cardinal directions are viable. Occasional diagonals are fine, but give plenty of time to react and recover.<br />&#8227; All note positions viable here in any proportion. Top row notes are fine, but make sure the spacing is not tiring for the player.<br />&#8227; Any color, any lane is fine. Always provide enough reaction time before a *true* crossover where the player’s arms have to physically cross over each other.<br />&#8227; Flow is critical unless you have an extended break. Try to cross the parity line with every swing.<br />&#8227; Most emphasis options are available, including inverted doubles with sabers going opposite directions. Stacks and sliders are fine, but keep them two notes long and don’t overuse them.<br />&#8227; All obstacles are fair game, but be wary about creating vision blocks. |
|   Normal   | &#8227; All cardinal directions are viable. Diagonals are not recommended for this level. All side notes should be treated as forehand hits.<br />&#8227; Notes should lie mostly in the bottom row. Use the middle row as a flourish for emphasis. Use the top row sparingly with dot notes only.<br />&#8227; Keep red notes primarily on the left side and blue on the right. Avoid crossovers entirely.<br />&#8227; Players will tend to reset after every hit, but you can introduce flow when the notes are too close together.<br />&#8227; Inverted doubles are manageable, but don't overuse them. Stacks and sliders should be scarce.<br />&#8227; If obstacles are used, they should be easy to avoid. You can sprinkle in notes simultaneously, but give plenty of time to react and recover.                                                 |
|    Easy    | &#8227; All cardinal directions are viable. Diagonals are not recommended for this level. All side notes should be treated as forehand hits.<br />&#8227; Notes should mostly lie in the bottom row. Use the middle row as a flourish for emphasis. Use the top row sparingly with dot notes only.<br />&#8227; Keep red notes primarily on the left side and blue on the right. Avoid crossovers entirely.<br />&#8227; Knock yourself out with parity breaks. Players will reset after every hit.<br />&#8227; Avoid inverted doubles. Sliders and stacks are not recommended.<br />&#8227; If obstacles are used, they should be easy to avoid with no simultaneous notes.                                                                                                                                                                               |
<!-- markdownlint-enable MD013 -->

### Note Density

**NPS** is a measure of note density, or the number of notes measured within a certain interval of time. The NPS ranges for each difficulty will fluctuate depending on the map, but it is common to reduce the note density of each difficulty by **20%** or more as you work your way down the spread.

The table below provides a range of NPS values calculated from all base game maps, so you can use these values as a recommended baseline for where your values may lie. For more information on the typical NPS ranges across each of the base game maps, check out the [Beat Saber Map Analysis](https://docs.google.com/spreadsheets/d/13wyoviJAplYOrsMocOA7YNXJxVRHd74G7z4U2jhCZa4) spreadsheet.

| Difficulty  | NPS Ranges  |
|:-----------:|:-----------:|
|  **Easy**   | 0.82 - 2.20 |
| **Normal**  | 1.05 - 3.22 |
|  **Hard**   | 1.73 - 4.24 |
| **Expert**  | 2.42 - 6.49 |
| **Expert+** | 3.21 - 8.69 |

In general, the rhythm choices across the spread should fit the song. A 200 BPM speed map is going to have a higher note density than a 120 BPM dance map.

### Note Jump Speed

There are several terms related to the speed and readability of the map. These terms are all interrelated and are typically influenced by the song’s tempo:

* **Note Jump Speed** (NJS) is the rate at which blocks move down the track at the player. A higher value will make the notes move faster, while a lower value will make the notes move slower.
* **Jump Distance** (JD, also known as **Spawn Distance**) is a measure of the physical distance (in meters) that a note will travel to reach the player.
* **Half Jump Duration** (HJD) is a measure of time (in beats) from when a note spawns to when it reaches the player.
* **Spawn Distance Offset** (Offset, also known as **Spawn Distance Modifier**) is a modifier that directly affects the Jump Distance. A higher value will make the notes spawn further away from the player, while a lower value will bring the notes closer.

The following video demonstrates the effect of these values in-game:  
[YouTube](https://youtu.be/S70CDoWjdwk) | [Streamable](https://streamable.com/2l7fz9).

Changing the NJS or Offset values will modify the HJD and JD of your map. Community editors will show you how these values change as you make adjustments. Fine-tuned NJS and Offset are a matter of personal taste, so you may need to rely on trial and error to find values that work for you. For lower difficulties, always be wary about putting too many notes on-screen at once based on the values you choose.

The table below provides a range of NJS and JD values from typical community spreads, so you can use these values as a recommended baseline for where your values may lie.

| Difficulty  | NJS Ranges | JD Ranges |
|:-----------:|:----------:|:---------:|
|  **Easy**   |   10-12    |   27-30   |
| **Normal**  |   10-12    |   27-30   |
|  **Hard**   |   10-15    |   24-30   |
| **Expert**  |   12-18    |   24-27   |
| **Expert+** |   15-23    |   24-27   |

## Playtesting
Already mentioned in detail on the [Mapping Home Page](./#playtesting) it’s important enough to mention again here:

1. Test your own work early and often, especially when you’re just starting out!
2. If you can’t test your own work have a friend play it. Just remember that a friend may be more likely to say "that’s awesome, man!" than to give you honest advice and risk hurting your feelings... even if that’s what you need.
3. Even if you test your own work you can become "map blind" because you know it so well and may not see playability issues
4. Use the `#testplays` channel on BSMG wisely. There are experienced mappers who will play your pre-release map and provide constructive feedback. Sometimes there’s a LOT of constructive feedback and that’s ok. Those experienced mappers were once newbies with terrible maps themselves. If you’ve read and absorbed the info on this page you will be much better off!

**HAPPY MAPPING!** Visit `#mapping-discussion` on the BSMG Discord with questions!

## Credits
Content in this section has been derived from guides by [Awfulnaut](./mapping-credits.md#awfulnaut) and [Hexagonial](./mapping-credits.md#hexagonial).
