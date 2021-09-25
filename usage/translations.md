# Translations

## The easiest way to translate

{% embed url="https://www.youtube.com/watch?v=tVNj-bOXk\_E" caption="" %}

## How to add a new language

To add a missing language, login as admin, and go to Translations.

Then go to languages and click n "+ Add"

![Add new language](https://i.imgur.com/MjCXlQs.png)

Add the language you want

![](https://i.imgur.com/DgQo69W.png)

## How to translate an existing string

Login as admin and go to Translations.

There, the translations strings are grouped, or if not grouped they are in Single \( Single strings \). You can also use the search box to quickly found the string. Select the language you want to translate to.

Initially, "English" should be the default locale, since there we have all the strings, so you can translate from.

![Translations](https://i.imgur.com/J9ETvom.png)

![](https://i.imgur.com/Zhs6Wc3.png)

After you have located the string, you can click on the pencil button and add translation

## How to add missing translation

Some string may be missing from both single or grouped translations. To add missing translations

First, click on "+ Add" to add a new term

![](https://i.imgur.com/naRDxDS.png)

There enter the existing string \( String that you see on the site ex. Platform Fee\) and your desired translations.

![](https://i.imgur.com/zaB7LVU.png)

## Add language on the front page

The dropdown of languages you see on the front page and in the admin language changer

![](https://i.imgur.com/tmVHN6R.png)

Is controlled from Settings -&gt; Localization.

![](https://i.imgur.com/Nc5e8xA.png)

## Add language on the front page

The dropdown of languages you see on the front page and in the admin language changer

![](https://i.imgur.com/tmVHN6R.png)

Is controlled from Settings -&gt; Localization.

![](https://i.imgur.com/Nc5e8xA.png)

> Please make sure you have the following format. SHORTCODE,Language name for example

`EN,English,FR,French`

`EN,English`

`EN,English,FR,French,RU,Russian,ES,Spanish`

## Translate the front page

To work on translating the front page, log in as admin, and go back to the homepage, you have the option to edit the translatable strings in that language.

![](https://i.imgur.com/ESEH0Od.png)

## Missing translation after update

We are maintaining only the English language. And with each update, we may add new strings in the **en.json** or some file in the **en** folder. We list this in the list of updated files.

If you have your site translated into some other language, you will need to add these missing translations.

The easiest way to do that will be to switch the site language back to English. After that, go into "Translations" and select your language and group you need to translate. In most cases, you need to translate only the "Single" group.

The missing translations will show as empty. So make sure you translate them.

After adding the missing translation, you can switch to your language.

-- Another option will be to use a tool like PoEditor, where you can update en.json in order to maintain full translation.

## Multi language menu

In some languages like arabic, the characters take up lot more spaces. So the default table size count is not enough. [Here](https://cln.sh/St3NVI) is how to change it to text

