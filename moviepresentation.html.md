Director Changes in Blockbuster Movie Series
========================================================
author: "Tim Keele"
date: "4/25/2020"
autosize: true


Summary and Motivation
========================================================

This is a quick visualization of three movie series that spanned over a decade, and whose directors changed hands several times, and possible metrics of their success as taken from wikipedia.org. 

We have plotted the movies in the order they released against their worldwide box office incomes in USD.  We have then sized each point based off the movie's budget, a sometimes approximate value for which we used the average of the given range, and colored them based off their average review score from the Rotten Tomatoes website out of 10.  Finally, we colored the border of each point a different color for every different director in the movie series, so that the advantages of retaining a director for multiple movies, or changing directors after a flop, can be inspected.  

Movie Data Used
========================================================

Here is the movie data we aggregated from Wikipedia and Rotten Tomatoes for the Harry Potter, Lord of the Rings, and Spider-Man movie franchises.  We gathered an average rating out of 10, budget and box office return in millions. We also created a field indicating when a director in the series changed.  Finally, we used a vector of starkly different colors to indicate different directors in our plots throughout a franchise.  Note that we counted two directors in the Lord of the Rings trilogies, this will be explained.


```r
hp <- data.frame( rating = c(7.06, 7.21, 7.85, 7.45, 6.9, 7.12, 7.09, 8.34), budget = c(125, 100, 130, 150, 150, 250, 125,125), boxoffice = c(975, 879, 798, 897, 940, 934, 960, 1342), director=c(1, 1, 2, 3, 4, 4, 4, 4))

lr <- data.frame( rating = c(8.18, 8.49, 8.69, 6.55, 6.81, 6.28), budget = c(93, 94, 94, 180, 225, 250), boxoffice = c(888, 951, 1142, 1021, 958, 956), director = as.factor(c(1, 1, 1, 2,2,2)))

sm <- data.frame( rating = c(7.64, 8.3, 6.23, 6.65, 5.81, 7.67, 7.45), budget = c(139, 200, 258, 215, 247, 175, 160), boxoffice = c(822, 789, 895, 758, 709, 880, 1132), director = as.factor(c(1, 1, 1, 2, 2, 3, 3)))

dircol <- c("goldenrod", "pink", "cyan", "darkslategrey")
```

Harry Potter Film Franchise (Original 8)
========================================================

Here we look at the original eight movies in the Harry Potter film franchise, noteable for its frequent director changes and tone shifts in the series.  It was the most continusouly developed of the movies in this quick study, release a movie about every two years.




```
Error in file(con, "rb") : cannot open the connection
```
