# Spotify Data Analysis Project

This project involves collecting and analyzing data from Spotify using the Spotify API and combining it with additional datasets to create a comprehensive music database.

## Features

- Retrieves personal top tracks and artists from Spotify
- Collects audio features and track information for a large number of songs
- Combines Spotify API data with external datasets
- Categorizes songs into main genres based on artist genres
- Creates relationships between songs and artists

## Dependencies

- pandas
- seaborn
- matplotlib
- numpy
- scipy
- spotipy

## Setup

1. Install the required dependencies:
   ```
   pip install pandas seaborn matplotlib numpy scipy spotipy
   ```

2. Set up a Spotify Developer account and create an application to get your client ID and client secret.

3. Create a file named `callback.html` in your project directory. This file will be used to display the authorization code from Spotify after the user grants permission to the application.

4. Update the `client_id`, `client_secret`, and `redirect_uri` variables in the script with your Spotify API credentials. Make sure the `redirect_uri` points to the location of your `callback.html` file.

5. When running the script for the first time, you will be prompted to authorize the application. The authorization code will be displayed in the `callback.html` page. Copy this code and paste it back into the script when prompted.

## Usage

Run the Jupyter Notebook to:
1. Authenticate with Spotify
2. Retrieve personal top tracks and artists
3. Collect track and artist data
4. Process and combine data from external sources
5. Categorize songs into main genres
6. Export the processed data to CSV files

## Output

The script generates several CSV files:
- `my_top_artists_df.csv`: Your top artists and their information
- `my_top_tracks_df.csv`: Your top tracks and their features
- `tracks_df.csv`: Comprehensive track database
- `artists_df.csv`: Comprehensive artist database
- `artists_songs_df.csv`: Relationships between artists and songs

## Data Sources

1. Spotify API: This project primarily uses data fetched directly from the Spotify API. For more information on the Spotify API, refer to the [Spotify API Documentation](https://developer.spotify.com/documentation/web-api/).

2. Additional Dataset: This project also incorporates data from the "Spotify Dataset 1921-2020, 600k+ Tracks" available on Kaggle. You can download this dataset from:
   [https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-600k-tracks](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-600k-tracks)

   Note: You may need to create a Kaggle account to download the dataset.

## Note

This project uses both the Spotify API and external datasets. The external data may not be as up-to-date as the API data.

## License

[MIT License](https://opensource.org/licenses/MIT)
