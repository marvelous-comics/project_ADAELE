# Title :
Marvellous comics: mirror of society  
(Go to [Milestone 3](#milestone-3))
# Abstract
Superheroes and villains in comics can have a real impact on society. They’re supposed to represent what’s good and bad. Thus, the way the character is portrayed will have an influence on the reader. If for example all villains are part of the same minority, people will unconsciously see them in real life as bad people. Moreover, a character like Tony Stark could inspire people to study engineering. And these are just examples to illustrate the power comics can have on us.
We can thus study this choice of characters, how diverse it is, and if there is a tendency towards a specific portrait for superheroes and villains. 
# Research questions
- The choice of the characters in comics : gender, race, sexual orientation, education, geographic origin… 
- Evolution of the diversity of characters during the years
- Compare two major comic books editors : Marvel vs DC
- Number of appearance of a character: what characteristics are more likely to survive during the years
# Milestone 1
## Dataset
- On https://www.kaggle.com/fivethirtyeight/fivethirtyeight-comic-characters-dataset:
	- Marvel-wikia-data.csv
	- dc-wikia-data.csv
- On https://www.kaggle.com/dannielr/marvel-superheroes#marvel_dc_characters.xlsx
	- marvel_dc_characters.xlsx
- https://marvel.fandom.com/wiki/Marvel_Comics (1)
- https://dc.fandom.com/wiki/DC_Comics_Database (2)
## A list of internal milestones up until project milestone 2
- 07/11: Get a complete database: parsing and merging all the previously provided datasets 
- 14/11: Get a completely ready-to-use dataset
- 21/11: Get a general representation of the dataset
- 25/11: Deliver the milestone 2 with an almost totally analysed dataset and a draft version of the data-story we want to tell
- 11/12: Data visualization and good idea of the data story.
- 20/12: Final Report

# Milestone 2:
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

CLEANING:cleaning_project_ADAELE.ipynb

DESCRIPTION OF THE DATASETS: Marvellous Comics Notebook.ipynb

In this past weeks, we've spend a lot of time to parse the websites and cleaning the data and not as much as we wanted on exploring the data itself. However we've constructed good and solid guidelines detailled in Marvellous Comics Notebook.ipynb and we are still confident with this amount of data to construct a good data story.

# Milestone 3

Here we are, the datastory is finished. Follow this link and enjoy the datastory: [Marvelous Comics, a mirror of society](https://marvelous-comics.github.io). 

We've study mainly 5 differents aspects. The general portraits of character at Marvel and DC comics, the relationship between portaits and behavior (if they are Good or Evil). We've studied the diversity on the characteristic and also what characteristic make a character famous or forgotten. Finally we've studied the author and editor of both company, to see if there is a link between all the answer that we found, and the writers diversity themselves. 

## Datastory

To have a better a experience of the datastory, please download the font: [Komika_hand](https://www.fontsquirrel.com/fonts/komika-hand) and install it following the step on [mac](https://www.fontspring.com/support/how-do-i-install-fonts-on-my-mac), [Windows](https://www.fontspring.com/support/how-do-i-install-fonts-on-my-windows-pc) or [Linux](https://www.linux.com/tutorials/how-manage-fonts-linux/) for the installation. You don't have to do it, but if you are grading us, please do it.
The repository of the website can be found [here](https://github.com/marvelous-comics/marvelous-comics.github.io). 

## Repo contents
- **Notebooks html**: This folder contains all the notebooks in html format. This way, all the plots are displayed. Please refer to this folder to see all the results.
- **Notebooks ipynb**: This folder contains the following files:
	-  `parsing_project_ADAELE.ipynb` (ML 1): This notebook contains the code used for the scraping of the wiki Comics websites
	- `cleaning_project` (ML 1): This notebook contains the code used for the cleaning of the data
	- `Marvellous Comics Notebook.ipynb` (ML 2): This notebook contains a first data acquaintance.
	- `/Editors writers `: Contains the analysis of the writers-editors and some pickled data
		- `Editors_writers_analysis.ipynb`: Contains the analysis of the writer and editor-in-chief of both journals
		- `Editors_writers_plots.ipynb`: Contains the ploting of the analysis for the website
		- Some more pickle data...
	- `Longevity criterion.ipynb` This notebook contains the analysis of the famousness of the character, how we defined the metrics and how we separeted the characters in three groups. There is also a huge amount of plots for the website, such as for: general characterisics of the characters, longevity criterion, diversity and some histogram on some famous characters.
	- `Map Citizenship.ipynb`: Contains the plot of the map
	- `Behavior Analysis Notebook.ipynb`: Contains the analysis of the behavior (good, evil) characteristic and its plot for the website. The function of plotting are reused for some of the famousness analysis.
	- `/data_pickle`: Folder containing some dataset in a pickle. Used to have a nicer repository.
	- `/img` Contains some images that we saved during the analysis. They are not used on the website.


## Individual contributions

- __Ahmed Kooli__:
	- Scraped the data from the web (with Antoine)
	- Took care of the website
	- Wrote the datastory
	- Analysed the plots
    

- __Antoine Schmider__:
	- Scraped the data from the web (With Ahmed)
	- Data cleaning
	- Helped with the website
	- Plot the map
	- Writer editor analysis and plots
	- Researched for plotting library
    

- __Jordan Metz__:
	- Data cleaning
	- Analysis of the data:
		- General characteristic analysis and plots
		- Longevity and famousness analysis and plots
		- Diversity analysis and plots
		- Writer and Editor analysis
    
    
- __Pierre-Louis Gaudillière__:
	- Data cleaning
	- Analysis of the data:
		- Behavior (good, evil) analysis and plots
		- Plots for famousness analysis
