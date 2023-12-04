# swccgpt
The AI Star Wars CCG Rules Expert

## Public Files
### cardFacts.txt
This file contains all the card definitions and is used by the AI to answer questions about the game. It is generated by the generateCardFacts.js script.

### tournaments.json
This file contains all the tournament decklists from the PC website. It is generated by the downloadDecklists.js script.

### Other Files
All other files are generated by scripts.


## Setup
### Card Facts
`node generateCardFacts.js`
This will download the card definition JSON files, card images, and generate the cardFacts.txt file.

### Download Decklists
`node downloadDecklists.js`
This will download all tournament decklists from the PC website from the year defined in the constasnt "CURRENT_META_YEAR" (or null for all years)

### Download Card Images
`node downloadCardImages.js`
This will download all images for all cards locally.

### Scrape Tournament Data
`node scrapeTournaments.js`
Scrapes the PC website for tournament data and generates the tournaments.json file. This will eventually be a pre-requisite for the downloadDecklists.js script.
