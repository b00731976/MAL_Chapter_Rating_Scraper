# MyAnimeList Manga Chapter Ratings Scraper 
________________________________________________________________________________________________________

## See how readers react to your favourite manga throughout the chapters

![snk_spoilerfree.PNG](attachment:snk_spoilerfree.PNG)




This program is a combination of 3 scrapers that go through MyAnimeList (MAL) forums to get the average ratings, the total amount of votes and the standard deviations of a manga, per chapter.
________________________________________________________________________________________________________

### 1- First Scraper: MAL Chapter Links Scraper

The first scraper go through MAL forums directly to get the chapters. However, because the search engine of MAL is reeeeeallly bad, he has to go through every potential results related to the name of the manga and the amount of chapters.

### 2- Second Scraper: MAL Through Google Chapter Links Scraper

The second scraper go through Google for better search results: MAL's search engine is poor and sometimes will simply won't give you the search results you want. This 2nd scraper will only look at the chapters that the first scraper didn't get.

### 3- Third Scraper: Total, Mean, Standard Deviation Scraper

The third scraper uses the links to scrap for the total amount of votes and calculates the mean and standard deviation.
________________________________________________________________________________________________________

### Server Restrictions and What to Watch out for

* Because we are using Google's search results without the API, potential errors might occur if you look for a lot of chapters.
* The implementation of the third scraper is lazy. It doesn't use headers and cookies which means we must create timeouts between every scrap to limit server's restrictions. Restrictions might still occur.

* You must check how the manga is spelled (JP or EN, generally JP) before the input.

* You must include the total number of chapters up to date in the input.
