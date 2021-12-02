# linja wawa
*Linja wawa* is a [*sitelen pona*](https://en.wikipedia.org/wiki/Toki_Pona#sitelen_pona) font made by [nimi Elemenopi](https://www.reddit.com/user/ElemenopiTheSequel/) &amp; [jan Melon](https://www.reddit.com/user/just-a-melon). *Sitelen pona* is a writing system for the conlang [*toki pona*](https://tokipona.org/) which was created by Sonja Lang. This font is released under the [SIL Open Font License](https://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=OFL) which means it can be used, studied, modified and redistributed freely as long as they are not sold by themselves (see the OFL.txt file for the full license). The initial glyph designs were made by nimi Elemenopi in 2019 but were only made into an installable font in 2021. You can download the latest version, [linja wawa 1.21 here](https://github.com/janMelon/linjawawa/blob/main/font-files/linjawawa1.21.otf) ([ttf file here](https://github.com/janMelon/linjawawa/blob/main/font-files/linjawawa1.21.ttf)).

![initial design](https://preview.redd.it/zn4bnkom63e21.png?width=1920&format=png&auto=webp&s=55b431cb8078e52cccbcdcbf9f2c22f450439f51)

## Setting up the Font
After installing the font, turn on Kerning, all Ligatures, and the "use Contextual Alternates" option. In MS Word, you can find this option by either right-clicking and then selecting "font" or by pressing Ctrl+D. 

![font set up](misc/initial-settings.png)

## Using the Font
### Typing Basic Words
When you type a *toki pona* word, it will be automatically converted to its *sitelen pona* glyph. E.g. if you type the word "ale", then it will be converted to the *sitelen pona* glyph for "ale" which looks like an infinity sign ⟨∞⟩. Currently, all *pu* words and *ku suli* words are available in this font.

One-letter *toki pona* words, like "a", "e", and "o" will only be converted into their *sitelen pona* glyphs if you add a space after it or if you type the same letter twice. Otherwise, it will only show as a latin character. E.g. typing "e" will result in the latin character ⟨e⟩, but typing "e " or "ee" will give you its *sitelen pona* glyph which looks like a sideway double-chevron ⟨»⟩.

![basic words](misc/word-examples.png)

### Name Cartouche
Names in *toki pona* are written by putting glyphs inside a cartouche. The first sound of each glyph spells out how the name is pronounced. To start a cartouche, type a left square bracket ⟨ &#91; ⟩. Then, type an underscore ⟨ &lowbar; ⟩ to make the upper and lower lines of cartouche. Now you can type any *sitelen pona* glyph and it will automatically be put inside the cartouche. To close the cartouche, type a right square bracket ⟨ &#93; ⟩. E.g. "jan Melon" can be written as "jan &#91;&lowbar;ma&lowbar;ee&lowbar;li&lowbar;oo&lowbar;ni&#93;".

![cartouche](misc/cartouche-example.png)

### Extra Features
Some words, like "pi" and "tawa" can become containers for other words. Type a greater-than sign ⟨ &gt; ⟩ after the container word, e.g. "pi>", and then type two underscores ⟨ &lowbar; &lowbar; ⟩ to create an underline that extends the container glyph so that other words can be placed on it. You can also type a plus ⟨ + ⟩ sign instead of a greater-than sign.

![extra](misc/extra-example.png)

## How Does This Actually Work?
As you may have already guessed, the font works by ligature substitution (liga). If there is a series of specific characters, the computer will replace them with a single character that has been prepared previously. The name cartouche and the underline for container words work by kerning (kern) so that the distace between two consecutive characters is reduced, or in this case the distance is negative so the characters overlap. This was made using [FontForge (p.s. it's free)](https://fontforge.org/en-US/) and you can see the [FontForge sfd files for this font here](/fontforge-files). There are many tutorials out there; specifically I followed [this one](https://www.youtube.com/watch?v=UUUeogQAjv0) when working on this.
