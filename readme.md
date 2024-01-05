### Preface
WaniKani collection consists of 8881 notes and 12700 audio samples 
(at least 2048 individual characters). Each character is supplied with english meaning,
multiple on'yomi and kun'yomi readings, radical decomposition, meaning and reading mnemonics
as well as context examples.  
It has been originally ported from the site by 
[@adeckforanki](https://www.reddit.com/user/adeckforanki/) alone.

This repository exists in order to provide a better user experience, systematic documentation,
and [issue tracker](https://github.com/FredericaBernkastel/WaniKani/issues).

**Learning Kanji** expects one to already have familiarity with hiragana and katakana. 
This collection then takes place in following order:
1. Radical recognition
1. Kanji recognition
1. Kanji reading
1. Vocabulary recognition/reading

#### Additional features:
- Ability to choose from two voice actors (Kyoko: female, Kenichi: male)
- One of many things wanikani reviews have lacked is that you were not able to type the 
  readings you want in the box. In the kanji lessons mode you are taught one reading,
  and in review mode you have to type the "one reading". 
  Now you can type one or more readings. You can even type in them all to test your skills.
  
### Installation
Download latest `.apkg` file from the [release](https://github.com/FredericaBernkastel/WaniKani/releases) section, and import it in the program as usual.

### Additional configuration
- Open deck options, and decide learning settings. Following are preferred by the author,
  but you are free to experiment with them!
  - "New Cards" tab
    - Learning steps (in minutes): `1m 10m`
    - Graduating interval (days): `1`
    - Easy interval (days): `2`
  - "Display Order" tab
    - **New card gather order**: `Ascending position` **(requires Scheduler V3/Anki 2.1.49)**
    - New card sort order: `Ascending position` or `Card template, then ascending position` (first study recognition, then all readings)
  - "Advanced" tab
    - Starting ease: `1.5`
    - Easy bonus: `2.0`
    
- Decide preferred voice actor (the default is Kenichi, Tokyo accent, male). 
  In order to change it to female:
  - Click `Browse -> Note Types -> vocab Model -> Reading`, and then on `Cards...` button.
  - In opened window choose `Back template`, find `{{Audio_b}}` and replace the 
    letter `b` to `g`. Remember "b" as in boy for the male voice, and "g" as in girl for 
    the female voice.
  - Perform same steps for the `Recognition` note type as well.

- (Optional) Click `Browse -> Decks -> Wanikani Ultimate -> Fields...`. In opened window, select `sort_id` field, then enable `Sort by this field`.

#### Level system
If you are still having trouble with correct card ordering, Wanikani is split into **levels of complexity**. Starting from 1, and up to 60.  
In order to switch to this learning mode, follow these steps:
1. Open deck options, and set `New cards/day: 0`
1. Open `Deck -> Custom Study`. In the new window:
    - Choose `Study by card state or tag`
    - Click `Choose tags`, but skip new window without selecting any.
1. You will be moved to a new virtual deck called "Custom Study Session". Again, open options of this new deck.
    - Name: `WaniKani Level Session`
    - Search: `(is:new tag:level1) "deck:WaniKani Ultimate"`.
    - Limit to: `40` cards
    - Selected by: `Order due`
    - Reschedule cards based on my answers on this deck: `yes`
1. Click `Rebuild`

You will be able to study new cards from `WaniKani Level Session`, and review them afterwards as usual, in `WaniKani Ultimate` deck.  
Once you have finished first batch of cards, click `Rebuild` in the level session, which will fetch next one from the same level. Once you have done studying a level, increase the level tag in options.