Roll20Scripts
=============
This repository contains my various scripts, written in javascript, to enhance my roll20 game mastering.

These scripts are provided without license or warranty so feel free to use them in any way you like.

SpeakAs.txt 
	usage '!n {name} {/me|/w}{message}'
	
	This allows any player to speak emote, whisper etc. as anything else by typing !n {name} {message}
	eg "!n FluffyTheTerrible I speak all the things" will output 'FluffyTheTerrible: I speak all the things'

SpeakALanguage.txt
	usage '/w _{name} {message}'
	

	First, some background, all my languages in my campeign are represented as characters, controllable by
	the players that can speak it, second, they all start with '_'.

	My campiegn it is convention to whisper to the language that you are speaking to with
	causing the message to be delivered to all who 'own' the language.
	
	This script is designed to make it easier to see who is saying what in what language (even if you can't speak it)
	by automatically emoting 'says something in {languageName}' after any message whispered to a language.

SetCharacterAttribute.txt 
	usage'!attr {attrName} {"++"|"--"|"max"|variable} {optional message on reaching 0}'


	Sets the given attribute for the selected character (the one who's name is in the drop down box)
	"++" increments by one
	"--" decriments by one
	"max" sets the attribute to its maximum
	or, alternativly, a number can be supplied to set the attribute to.

	{optional message on reaching 0} - if the attribute reaches zero this message will be sent to the chat, can be an emote or whisper (ie. /w or /me)