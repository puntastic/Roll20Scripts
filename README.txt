Roll20Scripts
=============
This repository contains my various scripts, written in javascript, to enhance my roll20 game mastering.

Feel Free to use these scripts however you choose, but they are provide WITHOUT WARRANTY, if you choose to use them in your campeign
they could very well go very, very wrong. You have been warned.

All scripts are wrapped in try/catch blocks to prevent fatal errors from disabling all the custom scripts on the game's roll20 virtual machine.

!attr [attributeName] {++|--|max|[var]} [optionalMessage]
	Usage
		"!attr Ammo -- /me gun goes click"
		"!attr Ammo max /me reloads"
		"!attr HP -3"
	Notes
		Random values aren't implemented. However inline rolls should be able to be used in the 
		message... but I have not tested it.
		
		Will only modify the attributes set in your -character- which means that they will only be 
		updated on your token if the attribute is linked to said token.
		
		Case sensitive.

!n [characterName] [message]
	Usage
		"!n Charlie /me waves his hands ecstatically."
	Notes
		GM Only please, players can use it, yes, but don't.

/w [language] [words]
	Usage
		"/w _undercommon What?!"
	Notes
		You no Longer any need to use *language* when whispering to a language as you will automatically 		emote the language spoken to as though you had type "/me says something in [language]
