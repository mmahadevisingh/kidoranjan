# kidoranjan

This repo contains the source code for the prototype of kidoranjan app ,a kids entertainment android app with Content-based Recommendation using TensorFlow Lite and
Firebase. This is originally made for microsoft engage 2022. The app uses content-based recommendation algorithm, out of the 3 types of  recommendation engine algorithms- Collaborative, Hybrid and Content-based, i.e., it predicts the movies similar to the ones liked by user previously.This ensures that kids get their favourite content- out of numerous kid-movies,audiobooks and nursery rhymes.It is more efficient than the collaborative algorithm as it helps reduce the cold-start problem, i.e., as collaborative filtering is based on movies liked by previous users and response fully depends upon history, his preferences are not available in the beginning of app usage,hence,recommendations are not accurate. However, content-based approach is solely based on particular user attributes and movie attributes liked by that user. For example, if a kid is under 6 years  of age, he might rate nursery rhymes as his liked content. So, more nursery rhymes are recommended to him, giving him a more personalized experience. However, content-based recommendation engine has some drawbacks also, as the recommendations might not change, and user may not be able to view variations in recommendations, which collaborative filtering allows. Hence, hybrid technique is being used nowadays.

The model used in kidoranjan uses a Convolutional neural-network encoder (CNN): applying multiple layers of convolutional neural-network to generate an encoding of the user history analytics data. 

The app has a list of entertainment content for kids under the 1st tab. As the kids keep liking the content, the liked content is saved under liked tab. Recommendations appear in the recommendations tab accordingly.Also, it has a search bar to allow kids to search relevant content, if they do not like recommended content.

All data is stored using bigquery and recommendation is based on firebase analytrics data.Data is first loaded into pandas library via bigquery, which recieves analytics data from firebase as and when the app is used, and then,training and modeling of data according to ml- model algo is done using tensorflow and google colab and the model is stored in firebase.All thanks to google codelab and imdb data!!! THe languages used are kotlin,java and python.
  
Also, the app is solely made for kids entertainment, so that they get the best entertainment suited for their age group.

NOTE- THE ACTUAL SOURCE CODE IS CONTAINED IN START FOLDER OF THIS REPO. THE ORGANIZER IS REQUESTED TO IMPORT  AND  RUN THE START FOLDER CODE TO VISUALIZE THE FUNCTIONALITY ILLUSTRATED IN THE DEMO.
