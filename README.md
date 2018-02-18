# Python Tools
_a collection of python scripts which ease command-line work_


## Contents
* Gxep: grep, but for XML files

## To Dos:
* find better command-line arguments parsing module than argparse (in order to mimic GNU/Linux tools better) and use it in all the tools
* if you launch a tool directly by double-clicking on it in the file browser, it will start in GUI mode. if it does not have a GUI, it will show a graphical error message.
* find way to support command-line tab-completion

## Planned Tools
* make link: checks if given string is telephone number, url, email address, rss feed or file path and sanitizes the string and make a proper url out of it. can take multiple strings at once, a file or files, output to a file, open the URL(s) directly
* easy chmod: interpret permission string from ls as stanzas
* smart cd: cd to directory if given path is file
* download all files using url, looping through numbers
* verbose numbers and vice-versa
* manipulate tables
*		lines = rows or columns
*		remove lines
*		add lines
*		reorder lines
*		sort line
*		sanitize values:
			(select all numbers)
			(select lines/cells after specific pattern)
*			map values to different range
*			pad numbers
*		extract raw data
*
* convert files to windows/unix/mac line endings
* strip whitespace from files
* identify files and rename them according to their type
* generate list of trackers sorted by their ping speed
* generate links: mailto, tel, ...
* tool to create symlink bindings for steam games
* tool to create symlink bindings for common system-config-files
* CLI for own installer scripts
* generate combinations of given options
* own extensions for sublime text:
*	text-editor additions:
*		normalize space: remove additional spaces and replace them with one. "\s{2,}" to " "
*		normalize punctuation: remove unnecessary whitespace around punctuation and add correct one:
			"\s*([?.!,;:])\s*(?!\n)" to "\1 "
			"\s*([?.!,;:])\s*\n" to "\1"
*		normalize repetitions: remove unnecessary repetitions and correct them:
			"\.{2,}" to "..."(special 3 dot character here)
		normalize quotes: replace normal quote characters with fancy or locale dependent ones:
			"(["'])([^"']+)\1" to "“\2”"(or locale dependent quote characters)
*	if text is selected and the caps key is pressed, the text is converted to upper or lower case respectively
*	reindex list sublimetext addition
	"""
		FROM:
				1. bla
				1. bla
				2. bla
				4. bla
				6. bla
				3. bla
				9. bla
		TO:
				1. bla
				2. bla
				3. bla
				4. bla
				5. bla
				6. bla
				7. bla
		(also allows padding with 0's, choosing the start value and the step size (can also be negative))
	"""
*	regex extension to search for successive numbers
	"""
		WOULD MATCH:
				9. bla
				6. bla
				-------
				3. bla
				4. bla
				5. bla
				-------
				1. bla
				7. bla
	"""
*	specific standard regex expressions to ease searching: should either populate the history in the CTRL+F and CTRL+H screens or a menu which you call via a command: this presents you with a list of regex wher you choose one, this regex is then inserted into the search field of the CTRL+F/CTRL+H screen
*	automatic day/night theme: if time is past a specific defined time, a predefined, different theme is set to active: on_activated(view), set_timeout_async(callback, delay), run_command("select_color_scheme", "Packages/Colorsublime - Themes/Wildlife-Day.tmTheme")
*	expand lines: if you want to replace a words by multiple non-related words then the line is duplicated by the number of distinct strings and the respective word/phrase is replace by one of the target strings
	"""
		FROM:
				remove lines
				add lines
				reorder lines
		TO:
				remove rows
				remove columns
				add rows
				add columns
				reorder rows
				reorder columns
		(and vice-versa)
	"""
*	add tabs at the end of several lines to match them up
	"""
		FROM:
			Unmapped Pages|
			Current Page|
			Previous Page|
			Last Different Page|
			Pages Accessed|
		TO:
			Unmapped Pages			|
			Current Page			|
			Previous Page			|
			Last Different Page		|
			Pages Accessed			|
		(| symbolizes end of tabs)
	"""
* create web crawlers for common tasks: watching websites, downloading websites, social media feeds, DDOS a website or service, ...
* smarter regex: .+? or [^\n]+? are "less interesting" parts of a pattern. definitions like strings or specific, custom classes are more interesting. when highlighting, only the more interesting parts should be highlighted. better: ighlight whole match, but highlight more interesting parts more than the rest. also allow replacement/manipulation operations for those more interesting parts.
* smarter regex: support dynamically sized lookaheads and lookbehinds (`* + {} ?` and so on)
* create pkpass file from calendar event. can also just create the source files.
* have some support functions by default when launching python interpreter in terminal. see "using python as login shell"
* compress json(feed through json),html(???),xml(???),css(???),js(???),eml(???) files
* basic image manipluation tasks: scale/crop/flip/mirror/rotate image, black and white, add background (transparent, color, simple gradient), circumsize(remove equal amount of pixels from all edges)
* slice up images into chunks
* combine images as chunks to a bigger image

## Style
* There is a directory which contains the personalized scripts created by the tools
* secure environments?
* Those personalized scripts can be automatically saved to the correct folders if they are gonna be reused
* easy to setup reocurring runs of scripts
* the execution of a tool is already a script. meaning: if caled, this is considered as a personalized use. this ideology allows to also define repetitive runs for tools themselves
