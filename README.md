# LiChess Analysis Tool

### Purpose
This tool produces analysis and graphs for a chess user's game history with the intention of allowing a player to identify patterns and improve their gameplay. Also provides features such as a personal opening tree and win predictor.
<br><br>

### Setup
This tool currently works only with rated games, and the parsing works with LiChess' API: https://lichess.org/api#operation/apiGamesUser. The exact PGN download details are elaborated on in the notebook itself. It may or may not work with Chess.com's PGN download on rated games, which I have not been able to test.

This is run in an .ipynb file, so Jupyter Notebook is needed to run it. The .ipynb file should be in the same folder as the PGN files you will use as data. It will also be helpful to have Notebook++, but it is not necessary (the notebook explains why). 

Once you open the .ipynb file, there will be a few areas you will need to edit, for things such as inputting the PGN file name and your username. Once you have everything filled in once, make sure you save, so you can "Run all" on the notebook in the future with updated data.
<br><br>

### Demo
An HTML file (demo.html) is provided to show you what the output looks like on a sample user. 

A sample PGN and CSV(which is generated in the notebook) are provided as well.
<br><br>

### Introduction
The notebook is broken down into 9 sections.

The first section of the notebook converts your PGN file into a CSV file (table); once you have the CSV file, you do not need to run the first section until you get new data (or equivalently, a new PGN file).

The second section must be run every time the notebook is restarted. It reads in the CSV file and sets a lot of other important variables that will be used later on.

The analysis begins at section 3; while each section has its own separate topic/focus, sections 3 and 4 may be needed to run the other sections later on. The sections can be categorized as such:

Essential: Sections 3 and 4. Covers the most fundamental statistics for a user and their opening repertoire, the latter being the most important component of this notebook in my opinion.

Interesting: Sections 6 and 7. These deal with engine evaluations and clock times, and whil they can be argued to be equally as useful as sections 3 and 4, the PGN files do not guarantee that engine evaluations or clock times will be recorded for all games. In fact, it's been reported that only 6% of games come with an engine evaluation (To get an engine evaluation in the PGN file, you need to have clicked "Request a Computer Analysis" for that game on LiChess at some point).

For fun: Sections 5, 8 and 9. There is no analysis in these sections, but perhaps you can still take away something useful from them. They are interesting tools that each have their purpose outside of analysis, and hopefully you will have fun playing around with them as well.
<br><br>

### Contact
If you have any questions or suggestions, feel free to email me!
My email is kevingao26@berkeley.edu.

