# Bars.ai

Training a neural network to generate song-lyrics using a number of curated datasets containing lyrics from music artists.

by Alex Pinette, Milo Lani-Caputo, and Tamsin Rogers

## Scraping data

Using [Genius](https://docs.genius.com/), and [Spotify](https://developer.spotify.com/documentation/web-api/) Web APIs, we are able to get song lyrics as well as playlist and artist data.

### Getting started

First:

```bash
git clone https://github.com/alexpinette/Bars.ai.git
```

Then you are going to need to install the required libraries:

```bash
pip install -r requirements.txt
```

### Create your own API client

#### Genius

- Follow the instructions on [Genius API Documentation](https://docs.genius.com/) to get your own client_id, client_secret, and client_access_token.

- Then create a `genius_config.py` file with variables for your `client_id`, `client_secret`, and `client_access_token`.

#### Spotify

- Follow the instructions on [Spotify API Documentation](https://developer.spotify.com/documentation/web-api/) to get your own client_id, client_secret.

- Then create a `spotify_config.py` file with the variables for your `SPOTIPY_CLIENT_ID`, and `SPOTIPY_CLIENT_SECRET`.

### How to use

#### Data Generation

- Open the `data_generation_spotify` or `data_generation_genius` notebook. 

- Enter a playlist/album URL in the allocated variable for `data_generation_spotify`.

- Or, enter an artist name in the allocated variable for `data_generation_genius`.

- Other options are to choose from the already created datasets.

#### Training the Model

- Open the `model_generation_and_training` notebook.

- Input the currated .csv file in the associated variable.

- Run the notebook.

#### Generating New Lyrics

- Open the `lyric_generation` notebook.

- Update the associated variables with the correct dataset, and model.

- Create your own or allow the script to randomly generate a seed.

- Run the notebook.
