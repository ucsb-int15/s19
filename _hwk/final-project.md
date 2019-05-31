---
num: "final-project"
desc: "Final Project"
ready: true
assigned: 2019-05-31 13:00:00.00-7:00
due: 2019-06-12 23:59:00.00-7:00
---


# INT15 Final Project

The guidelines for the project are in the [int15-final-project.ipynb](https://int15.lsit.ucsb.edu/hub/user-redirect/git-pull?repo=https://github.com/ucsb-int15/s19-assignments&subPath=hwk/final-project/int15-final-project.ipynb) notebook.


## Datasets

Below is a list of vetted datasets along with a brief description.  We’ve also included some questions that you may want to answer.  You are not required to answer these questions and you are encouraged to propose (and answer!) additional questions.  If you can find additional data related to one of the projects below, you should feel free to use it, **making sure to cite  and link to the source of the data**.  You are not constrained to use only the data provided.

If none of the datasets below is of interest and you have your own dataset that you are excited to analyze, please check with Prof. K or Prof. Franks before **Wednesday, June 3** to get approval.

-----

### Firearm permits and background checks

* Dataset: <https://github.com/BuzzFeedNews/nics-firearm-background-checks>

The data in this repository comes from the FBI's [National Instant Criminal Background Check System](https://www.fbi.gov/about-us/cjis/nics).
> Mandated by the Brady Handgun Violence Prevention Act of 1993 and launched by the FBI on November 30, 1998, NICS is used by Federal Firearms Licensees (FFLs) to instantly determine whether a prospective buyer is eligible to buy firearms or explosives. Before ringing up the sale, cashiers call in a check to the FBI or to other designated agencies to ensure that each customer does not have a criminal record or isn’t otherwise ineligible to make a purchase. More than 100 million such checks have been made in the last decade, leading to more than 700,000 denials.
> The FBI provides data on the number of firearm checks by month, state, and type — but as a PDF. The code in this GitHub repository downloads that PDF, parses it, and produces a spreadsheet/CSV of the data. Click here to download the data, which currently covers November 1998 – April 2019.

-----

### Analyzing OKCupid Data

* Dataset: <https://drive.google.com/drive/folders/1JxoceEaD97fJEQSICeILb440l5UFw_B1?usp=sharing>

Take an in-depth look at the world of online dating through this dataset! This dataset is a set of anonymized data from the popular online dating site, OkCupid.

Suggested directions:
* Where is OkCupid Popular? What kinds of places does online dating seem to thrive? Create a spatial visualization of the data.
* How does the population of the online dating world compares to the world population? What are the demographics?
* Prediction: Based on any demographic indicator, can you predict more information about the person in the online dating pool?
* PCA: What are the principal components in determining whether a person is single or not?
* Regression: Can you fit a model that predicts something about a person based on income, body type, offspring, orientation, pets, or other factors?
* Discuss the ethics of this dataset. Is the publication of this data ethical? Does it matter that the dataset was collected without the users' consent if these data are public?

-----

### Baseball Data
* Dataset: <http://www.seanlahman.com/baseball-archive/statistics/>

<https://www.baseball-reference.com/>

These datasets cover 1871-2018 batting/pitching stats for baseball (covers both players and teams) with plenty of metadata. Possible areas of exploration could include player performance comparisons with a visualization of player success over time (measures of success include, home runs, wins, salaries, etc.)

The data is separated into different files with different themes, so students need to look at the files and decide which to analyze and which topic to focus on. Very friendly for insights via regression.
 
----- 

### Spotify & Pitchfork Reviews

* Dataset:  <https://drive.google.com/drive/folders/1JxoceEaD97fJEQSICeILb440l5UFw_B1?usp=sharing>

(Warning: large files!)
 *  acoustic_features.csv (63Mb)
 *  albums.csv (42Mb)
 *  reviews.csv (86Mb)

Spotify is a leading music streaming service that collects a lot of data about the music they have access to, and user's listening habits. Take advantage of their data-driven approach by looking at the EchoNet information about some of the top tracks on the billboard 200. You could even use the EchoNest API to see what kind of information is available about your favorite songs! More information about working with EchoNest is available here: <http://static.echonest.com/enspex/>

Spotify collaborates with EchoNest to understand music at a deeper level by breaking down songs to "acoustic" information. A look into the `spotify_echonest` DataFrame reveals what kinds of data that consists of. It ranges from things like "danceability" and "energy" to more conventional music theory ideas like tempo and key. This gives us numerical power in analyzing music easily! We can use this information to see what kind of music tends to be successful, and what trends we can aim for if we wanted to make the next summer playlist.

You can also integrate [Pitchfork](https://pitchfork.com) music reviews.

Possible directions:
* PCA: What particular attributes make a song popular on the billboard 200?
* Prediction/LR: Can you make a model that can predict how successful a song will be on the billboard 200?
* Questions: What albums have been outstandingly successful? ie maintaining a high position on the top 200 for a long time? 
* What genres seem to dominate the top 200? What genres get the best critic approval?
* Do popular songs seem to get high critic approval? Do critics seem to agree with the popularity of an album?

-----

### Crime Statistics and Police Data
* Dataset for Seattle: <https://data.seattle.gov/Public-Safety/Seattle-Crime-Stats-by-Police-Precinct-2008-Presen/3xqu-vnum>

Possible questions:
* How did crime in Seattle has changed over time? Are certain crimes are trending upward? Are certain precincts are experiencing more crime than others (and how has that changed over time)?

* Compare it to other cities, such as 
  * Berkeley: <https://data.cityofberkeley.info/Public-Safety/Berkeley-PD-UCR-Annual-Part-I-Crimes/efkp-2py4>
  * ...

