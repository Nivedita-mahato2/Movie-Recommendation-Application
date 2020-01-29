# Movie-Recommendation-Application
CA675 Cloud Technologies Assignment 2

YouTube Link for working demo: - https://www.youtube.com/watch?v=Yx5t_bTqoak&feature=youtu.be


Introduction:
We have created a Movie database web application. The web application consists of four pages described below.
Home Page:
The page displays the top 10 rated movies along with five similar movies (used Correlation machine learning algorithm).
The page consists of 2 buttons: Recommendation and Browse Movies.

Browse Movies Page:
User can filter movies on this page based on three parameters, i.e. Year, Genres and Ratings. After selecting the filters and clicking on submit button, it will display the list of movies on the third page.

Display Movie List Page:
This page will display the movies list consists of Movie Name, Rating, Year, Genres to the users based on the filters applied on the browse page.

Recommendation Page:
This page is divided into three sections.
Section -1 will display the top 10 users and movie recommendation based on user selection. (Used K nearest machine learning algorithm)
Section -2 will display the percentage distribution of genre’s based on Movie Count.
Section -3 will display the number of movies for each genre from the year 2000 – 2018.

Motivation:
Selecting a movie to watch is an enormous task and many people find it challenging to select a particular movie from such huge pool of movies. Therefore, a movie recommendation system is extremely important given the massive demand for personalized content of modern consumers. An example of a recommendation system is as below:
User A watches Avengers: Age of Ultron and Iron Man 3.
User B does search on Avengers: Age of Ultron, then the system suggests Iron Man 3 from data collected about user A.

Choice of Technologies:
Google Cloud Platform: Used Google Cloud Platform for processing the data.
Anaconda & Jupyter Notebook (Python): Python for Machine learning algorithms such as K Nearest Neighbours (KNN) and Correlation algorithms for training the data.
Eclipse IDE: For the creation of Google App Engine Standard Java Application using Maven dependencies Eclipse IDE is used.
HTML/CSS: Hypertext Mark-up Language is used for defining the content of webpages. CSS is used for styling the appearance of content and webpages.
JavaScript: To program the behaviour of the web pages.
Java: Created servlet-based application to perform the dynamic action to the webpages and also used for the jdbc-bigquery database connection.
Excel and Google Refine: Data Cleaning was done using Excel and Google Refine.
Tableau: The data was analysed using tableau. The recommendation data is also displayed using Tableau Public.

About Data: 
We have considered a dataset of IMDb (Internet Movies Database) from the year 2000 to 2018, which consist 10,683 movies and 374,711 movie ratings records and have the following parameters:
MovieId
Title of Movies
Genre of those Movies
UserId of Users providing rating to those Movies
Rating of Movies 
Timestamps

About Processing:
The processing of data took place in 3 stages:
Using Excel and Google Refine, data was cleaned and all the null fields were removed. The format of the movie title was corrected as it consisted Junk characters. Title name and Years are split using Excel. 
After cleaning the data, it was loaded to Google Bigquery as Movies.csv and Ratings.csv. 
The data received from the Movie Recommendation model built by Machine learning algorithm was then saved in excel and was also pushed to Google Bigquery Database.

Related Work:
James Le (April 22, 2018) The 4 Recommendation Engines That Can Predict Your Movie Tastes [online] Available at https://medium.com/@james_aka_yale/the-4-recommendation-engines-that-can-predict-your-movie-tastes-bbec857b8223
Don Reisinger(March 19, 2009) Top 10 movie recommendation engines [online] Available at https://www.cnet.com/news/top-10-movie-recommendation-engines/Lops, Pasquale, Marco De Gemmis, and Giovanni Semeraro. "Content-based recommender systems: State of the art and trends." Recommender systems handbook. Springer, Boston, MA, 2011. 73-105.
Wei, Jian, et al. "Collaborative filtering and deep learning-based recommendation system for cold start items." Expert Systems with Applications 69 (2017): 29-39.
Ekstrand, Michael D., John T. Riedl, and Joseph A. Konstan. "Collaborative filtering recommender systems." Foundations and Trends® in Human–Computer Interaction 4.2 (2011): 81-173.

Challenges Faced:
We faced multiple issues in the process of making our application robust:
Connecting BigQuery database to Eclipse IDE. The connection was established successfully by creating JSON for Google account credentials.
Even after deploying the project to Google API engine, we were not able to load our webpage. We resolved this issue by using a Cloud API. To access the Cloud API, we created a Google App Engine Standard Java Project in Eclipse IDE so that multiple resources could be used which are provided by Google Cloud Platform.
Issues were faced in Maven dependencies and we added required dependencies in POM.xml to make the project executable.

