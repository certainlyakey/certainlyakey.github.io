---
layout: post
title: Game studies
excerpt: Final assignment — Game concept
course: Basics of Game Theory and Design
---

#Goal

This is a concept for a learning game codenamed Game-of-type. It's related to typography which is the art of designing and arranging type and text layouts for readability and style. I got an initial idea for such a game when I worked as a teacher of typography in the design department of a university. Students aren't particularly good with one area of typography which is the structure or architecture of type (meaning typographic symbols, mainly characters). 

There is a variety of components in graphical representation of a letter — terminals, counters, apertures, and so on. They are particularly hard to learn. The reason behind this is that the words in the glossary of letter architecture components are old — because of the 5 century-long tradition of calligraphy, typesetting and designing type — and numerous enough to often avoid connotations with other areas of knowledge. Many terms have been taken from the technological and highly specialized practice of printers and typesetters and thus are sometimes too metaphorical to be learnt easily (say, bowl, leg, shoulder etc.) or taken from another language (Italian and French as an example).

#Audience

This is the rationale for a game that would afford learning of the typographic glossary in a quick and not boring way. It gives an extrinsic motivation for learning without having to memorize the quite big list of terms. The audience for this is the typography classes students and basically anybody who's interested in type — that includes practitioners or students of type, print, web, UI design and so on. A player as a consequence of a play might learn the vocabulary of terms both in English and Russian and be able to name all of the components of any given character of any given font or font style. Even though the game is intended primarily for people who are not experts of the field it might be still useful for experienced non type designers who don't use the type vocabulary often (as in the latter category probably only type designers would fall). This game is also intended as an educational supplement to a real typography class, but its context of use is more out of class, such as random playing on the go or at home.

#Rules, roles, resources

The rules of the game are relatively simple. It's a screen-based game. The game is played by one player. On launch player has a random phrase presented before him and a list of type terms that is compiled from the elements that are actually present in this phrase. The phrase can come from a pool of 3x5=15 consecutive difficulty levels. The difficulty of each level is composed from two factors: the phrase length and the complexity of type with which the phrase is set. So with each move onto next level (which might happen every three succesful rounds) either the phrase becomes longer or the font graphics more complex (we can begin for instance with Helvetica and finish with highly sophisticated typefaces such as Zapfino). It's also possible that on the higher level the font size becomes a little lower though it shouldn't impede accuracy of clicking.

The game can be played with or without time limit, in the latter case the levels come up completely randomly on any successful round or by pressing a button without any progression. In this case it's also possible to enter your own phrase (with a maximum length limit). Each successful hit adds up a certain amount of time that allows to have more time on thinking and choosing. The resources that can be considered here are time (if the game is played with time limit), the number of terms, and the number of characters in a phrase. The phrase itself and the terms list can be considered a game object.

#Core mechanic and game dynamics

Then player must indicate where all of the listed terms are located in the characters of the phrase by clicking on a term, then on respective parts of the characters. Because one element might appear on many characters in a phrase (for example serifs in a serif font would be really frequent) a click on any of those would count and "deactivate" the term in the list. The game has linear dynamics which means that it will progress linearly as the player advances through the difficulty levels.

Different types of type elements can be given different value and thus for example may extend time limit by different amount of time. The round is won if all the listed terms are guessed correctly (within given timeframe) and is lost if less than 70% terms are guessed right. If an element is guessed incorrectly then it is highlighted with color briefly on the phrase anyway — it's an educational game and a player should learn something even if he loses. 

#Elements

Important game elements here are:

- time — it creates a challenge even for experts of type or experienced players;
- progress — as difficulty progression goes further player may find himself discovering unfamiliar components of type such as various diacritics or calligraphic elements;
- style — every game on type, especially puzzle games that are driven by a learning goal, should be appealing visually. That's why the implementation of such a game should be minimalistic in style, have pleasant aesthetics and have as few interactive features in its interface as possible. It also should maintain a serious tone in the style and shouldn't be overly "fun" in its design;
- exploration — a player is able to take his time, explore font features, and learn without any penalties. He's also able to study on a material provided by himself (the ability of typing your own phrases and playing on the basis of that).

#Platforms, controls, distribution

The game is intended to be either web-based or mobile app based. The reason behind this is that its simple mechanic is okay for quick introduction into the typography terms or for playing a 5-10 minute session on the go. It's meant thus to be controlled with mouse, touch, or possibly keyboard. As this game is a learning game it'll probably be distributed around for free as a link to a website or a application.

Here are some screenshots of Game-of-type graphical prototype:

![Screenshot 1](/images/game-of-type/1.png)
![Screenshot 2](/images/game-of-type/2.png)
![Screenshot 3](/images/game-of-type/3.png)