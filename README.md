
# Magic Research 2 Public Translation Project

**It seems that mcolotto’s [original project](https://github.com/mcolotto/magic-research-2-translations) is no longer active. This is my attempt to revive it and to compile the existing translations available for Magic Research 2**

--------------

This repository is meant to be used as a way to organize crowd-translations of the game Magic Research 2. Please read on to find out how to contribute!

## Translation Status And Credits

[![Translation Status](https://weblate.mystikal.it/widget/magic-research-2/game/multi-auto.svg)](https://weblate.mystikal.it/engage/magic-research-2/)

I've gathered the available translations file on the web for this game. They will be used as a starting point for this project:
* English (United States): Done (N/A, original language)
* Russian: FArgus (Found on Discord)
* Chinese (Traditional): pierre654852 (Found on Discord)
* Chinese (Simplified): [@JingruiChen](https://github.com/chen-assert)

This readme is mostly copied from the one made by mcolotto

## Magic Research 2 Translation Guide

This guide is intended as a way to provide a custom translation for Magic Research 2. It is meant for those who would like to translate the game.

**Caution: As this is a text-only game, there is inevitably big, big spoilers for the _entire_ game inside the translations file. If you'd like to experience the game at its fullest and you're able to understand English, I suggest you complete the _full_ game first before starting to translate. Translate it at your own risk!**

You can help translate this game using [this weblate project](https://weblate.mystikal.it/projects/magic-research-2/) or by contributing to this github directly. 

If you don't want to use Weblate, you can follow mcolotto original guide:

The process essentially is as follows:

1. Start with the `base-translations.json` file in English as a base. This file is a key -> value object where the first string is the key (always the string in English) and the second string is the value (by default, exactly the same as the key).
2. Edit the values for the target language.
3. Once you are done editing, load the file into the app via the Options menu.
4. Restart the app.
5. The app will now use the translations.

If a key is not found in a translation file, the game will use the English as a default.

The strings are pretty special in the sense there are many special characters:

- `\n` is a new line (not always supported, but if you see it in one, it probably is).
- Many of the strings are in Markdown format. Refer to the Markdown syntax for more details.
- Double braces inside a string (for example: `"**New spells learned:** {{newSpellsLearnedText}}"`) indicate parameters and they will be replaced when playing the game with some other string.
- Some things wrapped between colons (for example: `"+10:attack:"`) will be replaced with a picture of an icon. Because those are identifiers, if you want the icon to appear, you will want to keep that piece intact.
- Finally, in some cases, you will see some complex pieces which are wrapped first with `^^`, followed by `<>` (for example: `"Can be used ^{{times}}^<{{explanation}}> times per combat"`). These are the underscored tooltips that you see throughout the app. When displayed, the text shown will be what is between `^`; it will be underlined, and if a mouse is hovered over the text, or the text is pressed in mobile, it will show a tooltip with what is in between `<>`.

As of the time of writing, there are about 4000 strings. Some of those may require little or no changes between most languages as they are almost entirely tokens, while some other individual strings are full paragraphs of story. There is no structure or context for the strings - it isn't planned as it was already a monumental undertaking.

## How to Contribute

You are free to create your own translations and distribute them on your own if you'd like. However, because translating the game is a very big task due to the sheer amount of strings, this repository also serves as a way to organize and share the load with others.

You can help translate this game using [this weblate project](https://weblate.mystikal.it/projects/magic-research-2/). 

If you don't want to use the Weblate Project, you're free to contribute by committing to this repository directly by following this guide:
1. If there is no translation file for your locale, please create one by copying `base-translations.json` and committing it to the folder `translations` using the [ISO-639](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) 2 letter language format as a file name (for example `fr.json` for French). If your language have different writing system, you can add the [ISO-15924](https://en.wikipedia.org/wiki/ISO_15924) code to the file name (for example `zh-Hans.json` for Simplified Chinese). If your language have multiple version based on the country, add the [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1) code to the file name (for example `pt-BR.json` for Brazilian Portuguese)
2. Once that is done (or if there already was a translation file), feel free to edit the file at leisure with any tools. Editing the file directly in this repository might be the best way to start. 

There is a channel in the official [Magic Research Discord server](https://discord.gg/bPhGsaqR9d) called `#mr2-translations`. It can be used as a venue for discussion and collaboration if needed.

## Questions, Suggestions, Etc.

Note from developer: It is my first time trying to build a translatable game from scratch, so chances are there are many, many things we could improve about this, especially in terms of process. There are also likely other elements in the app that will need attention for some locales: things like RTL, number formatting, etc. I am open to suggestions on how best to work. The best way to reach me is likely through Discord as mentioned above, in "How to Contribute".

## AI Usage

Some translation have been made using Gemini/ChatGPT. The Weblate project uses DeepL for automatic suggestion
