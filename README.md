# Movie-Recommender

![269458670-d63db2b8-94a0-448c-8020-2f797d7cc318](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/d328f75a-1d20-48c9-ba3d-747b70e8e0dc)












# Movie recommendations project 

## Project Description:
### Overview:
The Movie Recommendation Web Application is a data-driven project designed to assist movie enthusiasts in discovering new films similar to their favorite titles. Leveraging data from Kaggle, this project involves data preprocessing, feature engineering, and machine learning techniques to deliver personalized movie recommendations to users through an intuitive web interface.
### Key Project Steps:
#### 1) Data Import and Cleansing:
(i) The project begins by importing movie-related data from Kaggle, which includes information about movie_id, titles, overviews, genres, keywords, cast, and crew.

(ii) Data cleansing techniques are applied to handle missing values, duplicates etc,ensuring the quality and consistency of the dataset.

#### 2) Feature Engineering:
To improve the recommendation process, key information from various columns, including overview, genres, keywords, cast, and crew, is combined to create a new composite feature called "tags." This step enriches the dataset with valuable content information.
#### 3) Text Preprocessing:
Natural Language Processing (NLP) techniques are employed to preprocess the text data. This includes stemming using NLTK, which reduces words to their base forms, improving text similarity calculations.
#### 4) Vectorization:
Scikit-learn's vectorization methods are utilized to convert the text data into numerical format, making it suitable for machine learning algorithms. This step transforms the "tags" column into a numerical representation.
#### 5) Cosine Similarity:
The heart of the recommendation system is built on cosine similarity. Using Scikit-learn's cosine similarity function, the project calculates the similarity between movies based on their "tags."
#### 6) Recommendation Engine:
A recommendation model is developed using the cosine similarity scores. When a user inputs a movie title, the system identifies the top 5 movies that are most similar to the user's input.
#### 7) Web Page Development:
(i) The recommendation model is integrated into a user-friendly web application using Streamlit, a Python library for creating interactive web apps.

(ii) The web page provides a search box where users can input a movie title of their choice.
#### 8) Deployment:
The Movie Recommendation Web Page is deployed on render.com .

## Objective:
(i) Develop an accurate and efficient movie recommendation system.

(ii) Provide users with personalized movie recommendations based on their input.

(iii) Enhance the user experience by creating an intuitive web interface.

(iv) Deploy the web Page to make it accessible to a broad audience of movie enthusiasts.















## 🛠 Tools used


Pyhton, Nltk , Sklearn, Streamlit
## Data Cleaning &  Feature Engineering  :
(i) Checked and removed null,noise,duplicates.


![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/a7547add-f7db-4e56-a5f5-82ab10900f1d)





(ii) Extracted the desired values from each column by appliying functions on the columns which were in the form of dictionary.


![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/26c89ee8-3cc5-495e-b6de-2b7719cafd0d)




![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/ddcb0c3c-02df-4821-bf87-91a9e172a675)








(iii)  meticulously amalgamated the contents of these columns, ingeniously crafting a novel column dubbed 'tags.' This involved uniting all the extracted values with spaces and then uniformly converting them to lowercase



![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/55277270-6441-496d-ba47-50319a817452)







 
 ## Model Building 
 (i) The installation of 'nltk' was followed by the importation of the 'PorterStemmer' module. Stemming, a crucial data refinement process, was then skillfully applied to reduce words to their base forms.
 
 
 
 
 ![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/0b5a987a-b898-42d7-b7d6-2a937f9b0f62)








 
 (ii) Installed 'CountVectorizer' from 'sklearn' with 'max_features' set to 5000. Created an object named 'vector' using 'cv.fit_transform' to transform the 'tags' column in our dataset into a numerical format.





![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/3e306947-13b2-455d-9237-ba18fe13c879)






 
 (iii) Incorporating the power of 'cosine_similarity' from the 'sklearn.metrics.pairwise' library, this code elegantly measures the similarity between movies by analyzing their content. By constructing a similarity matrix, the 'recommend' function is equipped to accept a movie title as input. It meticulously identifies the movie's index in the dataset, subsequently retrieving the top 5 most akin movies. These recommendations are thoughtfully curated based on the movies' cosine similarity scores, empowering users to explore cinematic gems aligned with their unique content preferences.

 





![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/3af5b160-28db-43cf-8ada-f00d2e8bca79)











![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/07123d2e-3f47-4e69-b164-d03228cd52e3)










 (iv) Saved the movies and similarity in a folder with the help of pickle.





![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/f451df9c-b129-4944-b3a8-d2a29da0750d)








 

 ## Webpage building
 A Movie Recommender system was created using Python and Streamlit. The code utilizes a dataset of movies, loaded from a 'movies_dict.pkl' file, and a precomputed similarity matrix from 'similarity.pkl.' The heart of the system is the 'recommend' function, which takes a user-selected movie as input and returns a list of the top 5 recommended movies based on similarity scores. The Streamlit-based user interface allows users to choose a movie from the dataset and click the 'Recommend' button to instantly receive personalized movie suggestions. This project offers an engaging and user-friendly way to explore movie recommendations.










![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/e36583cb-2bac-4a97-ac86-9cafff8f7e7c)








![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/4ade356a-2d2e-4eb1-a2bb-3a4283a49ba2)



# Here are some screenshots showing how it works 








![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/64e2c95a-b50c-4ed1-a572-ebe34001f654)




![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/a35ac20d-8a96-4334-bff4-b303abed7558)










![image](https://github.com/aayushkataria123/Movie-Recommender/assets/137820574/55c65b9c-d56d-45d0-81b2-dcdf58e25b1d)










# Problems Faced
### (i) Selecting important keywords from the columns
### (ii) Determining the most effective method for measuring movie similarity.
### (iii) Identifying the approach to building the webpage.
### (iv)  Exploring the process of deploying our webpage.  
