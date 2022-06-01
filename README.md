# Finding-similar-Net-Energy-Demand-Profiles
Using wind and demand profiles to find similar days to the following days forecast which can help give an expectation

## Usage

Uses data to create a plot of net demand for each day in dataset and does some processing on these plots and saves as image. 

Image then converted to tensor and used to train an Autoencoder to extract the important features for each day. 

These embeddings then saved in a nearest neighbours classifier. 

When forecast for following day ran through Autoencoder and classifier it will return the most similar days and calculate the root mean square percentage error to identify how similar the returned days are to forecast.
