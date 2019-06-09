# spotify-recommendations

This app uses the Spotify for Developers API set. If you want to play around
with this yourself, first log in at their [developer's home page](https://developer.spotify.com/dashboard/applications) and create a new app. Make note of your Client ID and Client Secret, as you will need them later.

### Setup
If you run this app with Python3, make sure to replace `pip` with `pip3`.

```
pip install numpy pandas spotipy matplotlib
```


### Scopes
Scopes are Spotify's way of ensuring third parties only get to see the
information you open up to them. If you want to alter any of them, a list can
be found
[here](https://developer.spotify.com/documentation/general/guides/scopes/).

### Authentication
To be sure you are authenticated, you need to whitelist your callback URI into
the Spotify dashboard. You can do this by clicking `Edit Settings`.

### Things to Consider
It is important to think about how you would like to train your data. Do you train on the songs you like (giving them a positive score) and specify songs you dislike (giving them a negative scoring), or do you a assume all the songs you haven't trained on are defaulted at a negative score? The latter may be more interesting, but makes the training a little more complex. Therefore, on this first iteration, I have decided to specifically note what songs are classified as negative. Over time I would like to make this a little more sofisticated however.

I see this project becoming interesting when a user can give a specific dataset to train on (say, make "Recommended For You" playlists on specific moods they are in). 
