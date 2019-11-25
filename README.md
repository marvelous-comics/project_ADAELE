# Title :
Marvellous comics: mirror of society
# Abstract
Superheroes and villains in comics can have a real impact on society. They’re supposed to represent what’s good and bad. Thus, the way the character is portrayed will have an influence on the reader. If for example all villains are part of the same minority, people will unconsciously see them in real life as bad people. Moreover, a character like Tony Stark could inspire people to study engineering. And these are just examples to illustrate the power comics can have on us.
We can thus study this choice of characters, how diverse it is, and if there is a tendency towards a specific portrait for superheroes and villains. 
# Research questions
- The choice of the characters in comics : gender, race, sexual orientation, education, geographic origin… 
- Evolution of the diversity of characters during the years
- Compare two major comic books editors : Marvel vs DC
- Number of appearance of a character: what characteristics are more likely to survive during the years
# Dataset
- On https://www.kaggle.com/fivethirtyeight/fivethirtyeight-comic-characters-dataset:
	- Marvel-wikia-data.csv
	- dc-wikia-data.csv
- On https://www.kaggle.com/dannielr/marvel-superheroes#marvel_dc_characters.xlsx
	- marvel_dc_characters.xlsx
- https://marvel.fandom.com/wiki/Marvel_Comics (1)
- https://dc.fandom.com/wiki/DC_Comics_Database (2)
# A list of internal milestones up until project milestone 2
- 07/11: Get a complete database: parsing and merging all the previously provided datasets 
- 14/11: Get a completely ready-to-use dataset
- 21/11: Get a general representation of the dataset
- 25/11: Deliver the milestone 2 with an almost totally analysed dataset and a draft version of the data-story we want to tell
- 11/12: Data visualization and good idea of the data story.
- 20/12: Final Report

# Questions for TAa
- How to scrape on different web pages (for example on one page, we have the names of different characters and each one has a specific page.)
- Is it possible to plot data in a really fancy way (custom histogram with characters instead of bars) ? 

# Update for milestone 2:
We've decided to parse again all the website (1) and (2) (i.e. the Marvel and DC wikia) to get our own and up-to-date database. We have now four differents files:
- One with all the Marvel characters (that we've limited to Earth-616 which is the mostly known Marvel universe, and still regrouping around 28000 characters).
- One with all the D.C characters.
- One with all the Marvel comics.
- One with all the D.C comics.
Since the creation and modification of each webpage is open to everyone, the cleaning part has been a bit tedious. At the end, we still have some missing values but they only represent a small part of the dataset. 
For the D.C characters, we were given whether a character is good or bad which is not the case for the Marvel ones. To solve that, we've decided to look at the appearances of each characters in each comic and if he was in the good ones ("Featured" or "Supporting" characters) or not ("Antagonist/Villains"). The characters can be also noted as neutral if they were in the "Other characters". Since anyone can edit the webpages, we've also decided to verify the correctness of the good and bad information in DC characters with the same criterion.
Finally, we've also decided to look at who is writing and editing the comics. This part needs to be more looked at to see maybe some characteristics of the editors and the writers. This will be quite easily done since we've stored their URL in our dataset.

You can find every parts in different notebooks:
PARSING: parsing_project_ADAELE.ipynb
CLEANING:
DESCRIPTION OF THE DATASETS:
