# Phase 1 Project: Movie Analysis 
## By: Rachel Eastman 
Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they do not know anything about creating movies. I am charged with exploring what types of films are currently doing the best at the box office. I must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.
I decided to review three different variables: genres, directors and writers, and most profitable time of year to release a movie.

## The Data:
The data I used for this project was:
-	Genres
      - [imdb.title.basics](https://github.com/rcasey106/dsc-phase-1-project-v2-3/tree/master/zippedData)
      - [imdb.title.rating](https://github.com/rcasey106/dsc-phase-1-project-v2-3/tree/master/zippedData)
   	- [bom.movie_gross](https://github.com/rcasey106/dsc-phase-1-project-v2-3/tree/master/zippedData)

-  Directors and writers:
      - [imdb.title.crew](https://github.com/rcasey106/dsc-phase-1-project-v2-3/tree/master/zippedData)
      
-  Profitable release months
      - [tn.movie.budgets](https://github.com/rcasey106/dsc-phase-1-project-v2-3/tree/master/zippedData)

## Methodology & Results:
To find the most profitable genres, I decided to merge all three data frames together to get all the data into one data frame. I then dropped the null values from the dataset.  I used the median because alt textthe histogram showed an abnormal distribution. I found the most profitable domestic and most profitable foreign genres.
![alt text](https://raw.githubusercontent.com/rcasey106/dsc-phase-1-project-v2-3/master/foreign.png)
![alt text](https://raw.githubusercontent.com/rcasey106/dsc-phase-1-project-v2-3/master/domestic.png)

To find the most profitable writers and directors, I merged the genre dataset with the crew dataset. I dropped the duplicates. Then, using descriptive statistics, used the mean to find the writers and directors with most profitable movies. 
![alt text](https://raw.githubusercontent.com/rcasey106/dsc-phase-1-project-v2-3/master/writers.png)
![alt text](https://raw.githubusercontent.com/rcasey106/dsc-phase-1-project-v2-3/b83143a58ddb8e0dd64cc301f305482775d26720/directors.png)
To find the most profitable months to release a movie, I created a new data frame to include the release date and worldwide gross. Once again, I used descriptive statistics to find the mean and median of most profitable months. I concluded that the summer months, specifically June and July, were the best times to release a movie.
![alt text](https://raw.githubusercontent.com/rcasey106/dsc-phase-1-project-v2-3/master/ww_gross_month.png)


## Discussion and Conclusion
I was surprised by some results, especially time of the year to release a movie, which was June and July.  I expected December to be more profitable than what the data showed
The most popular genres include sci-fi and adventure. This was not as surprising to me as most of the most popular movies of all time include some adventure in it. Movies such as Star Wars and Star Trek are also high grossing movies in the sci-fi genre.
The most profitable directors are Josh Whedon (Buffy the Vampire Slayer), Adam Green (Frozen, 2010), and Jennifer Lee (Frozen, 2013).
The most profitable writers are Joe Robert Cole (Black Panther), Warren Ellis (Iron Man 3)
And Steven McNiven (Logan).

## Final Recommendations:
1.	Recommend releasing movies in June or July
2.	Recommend Sci-fi and adventure movies, and avoid war and documentary movies
3.	Recommend using as Joe Robert Cole, Warren Ellis or Steven McNiven as writers and Josh Whedon, Adam Green, or Jennifer Lee as directors.
