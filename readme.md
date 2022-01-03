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
1. Download latest `.apkg` file from the 
   [release](https://github.com/FredericaBernkastel/WaniKani/releases) section, 
   and import it in the program as usual.
1. Click `Browse -> Decks -> WaniKani Ultimate`, and make sure that the cards are sorted by
   `Due` column in ascending order.

**Additional configuration**: 
- Open deck options, and decide learning settings. Following are preferred by the author,
  but you are free to experiment with them!
  - Steps (in minutes): `1 10 60 60 120 120 360 360`
  - Graduating interval: `1 day`
  - Easy interval: `1 day`
  - Starting ease: `150%`
  - (in reviews tab) Easy bonus: `130%`
- Decide preferred voice actor (the default is Kenichi, Tokyo accent, male). 
  In order to change it to female:
  - Click `Browse -> Note Types -> vocab Model -> Reading`, and then on `Cards...` button.
  - In opened window choose `Back template`, find `{{Audio_b}}` and replace the 
    letter `b` to `g`. Remember "b" as in boy for the male voice, and "g" as in girl for 
    the female voice.
  - Perform same steps for the `Recognition` note type as well.
    