# Whereabouts

A daily map game: guess the mystery UK town, city, village or county in six goes. **[Play it](https://maps.tristanhotham.com/whereabouts/)**

![Whereabouts](header.png)

## How it works

- Type a town and pick it from the list. Each guess shows how far away the mystery town is, which way to go, and how close you are (0% at 1,000 km, 100% when you get it).
- Every wrong guess unlocks a clue: its size; its sunshine and rain; house prices (or pay) and the Leave vote in its council area; the oddest thing about its council area; its county or council; and finally its first letter.
- Get it right, or run out of guesses, and the town appears on the map with what its name means, a shareable grid of coloured squares and arrows, and your stats.
- **Today's town** is the same for everyone each day. **Practice** gives you a random town whenever you like.

**Modes.** Pick Town, City, Village or County. Each has its own daily answer, streak and stats, and the daily list reshuffles each time it runs out.

- **Town**: daily towns are drawn from about 240 UK cities and towns of 40,000 people or more; Practice uses about 560 towns of 15,000 or more. You can guess any of about 3,000 towns.
- **City**: the UK's 73 cities.
- **Village**: about 1,200 daily villages of 2,000 to 5,000 people (2,500 for practice, from 1,000 people), England and Wales only. The sixth clue gives the distance and direction from the nearest town.
- **County**: England's 47 ceremonial counties and the council areas of Wales, Scotland and Northern Ireland (112 in all). Clues add up the figures for each county's councils, and the last clue names its neighbours.

London's boroughs are left out as answers.

## Files

- `index.html`: the game (one page, no build step)
- `towns.json`: answer towns and cities with their clues and name meanings, the list of guessable towns, and area labels
- `villages.json`: answer villages and the list of guessable places for Village mode
- `counties.json`: counties and council areas, their member councils, neighbours, clues and name meanings
- `map.json`: simplified council boundaries and the map projection
- `build.py.txt`: the script that builds `towns.json` and `villages.json`
- `county.py.txt`: the script that builds `counties.json` (Python; uses data from my Higher or Lower game and earlier studies)

## Sources and licence

Towns: OS Open Names and GeoNames, via my [Sun and Rain](https://maps.tristanhotham.com/sun-and-rain-uk/) study, and ONS built-up areas (2022) for populations, via my [post box](https://maps.tristanhotham.com/postbox-kings/) study. Weather: Met Office HadUK-Grid 1991–2020 averages. Council clues: the 66 measures in [Higher or Lower](https://github.com/Tristan-Hotham/higher-or-lower) (ONS, Nomis, Electoral Commission, Met Office and counts from my own studies). Council boundaries: ONS. Contains public sector information licensed under the Open Government Licence v3.0; contains OS data © Crown copyright and database right 2026; GeoNames (CC BY 4.0).

Name meanings are the usual explanations of common place-name elements; many names have more than one theory.

Code: MIT. Derived data: CC BY 4.0, keeping the attributions above.

Dr Tristan Hotham, independent researcher · 2026 · [tristanhotham.com](https://tristanhotham.com)

AI use: built with coding and drafting help from Claude (Anthropic). I reviewed and checked the data and text.
