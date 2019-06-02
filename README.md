# spotify-recommendations

This app uses the Spotify for Developers API set. If you want to play around
with this yourself, first log in at their [developer's home page](https://developer.spotify.com/dashboard/applications) and create a new app. Make note of your Client ID and Client Secret, as you will need them later.

### Setup
If you run this app with Python3, make sure to replace `pip` with `pip3`.

```
pip install spotipy
```


### Scopes
Scopes are Spotify's way of ensuring third parties only get to see the
information you open up to them. If you want to alter any of them, a list can
be found
[here](https://developer.spotify.com/documentation/general/guides/scopes/).

### Authentication
To be sure you are authenticated, you need to whitelist your callback URI into
the Spotify dashboard. You can do this by clicking `Edit Settings`.
