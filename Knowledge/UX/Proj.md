**I reviewed the features implemented, included an external Web API
and hope that this version incorporates more of course's topics,
while the idea might seem similar at first I consider it to
be much more complex**

Music listening tracker application v3

The application utilizes Spotify's API as well as has it's OWN database
for content that is not present on Spotify's servers.

Spotify's Web API allows to manipulate real data of real Spotify users.
This allows to retrieve information about currently played songs, user's playlists, create reports on user's activity and integrate user's account with
their Spotify account if users desire:
create and edit playlists, manage likes, save or remove albums/tracks,
control song playback and queue, follow artists/playlists/users.

Because of that security is a concern.

This web application allows users to register, log in, and track their listening
progress through albums, artists, and playlists.
The app is focused on helping users organize, log, and reflect on their music
listening habits, while discovering new music through community insights.
App includes data validation and different access levels.

The app analyzes registered user's listening activity and displays:
	- Listening history
	- Daily listening time (GitHub commit tracker style)
	- Genre diversity score
	- Recaps on favorite artists/songs/albums (This week/month/year etc.)
	- Achievements (e.g. "Listen to 10 albums from 10 different years")

All the activity is calculated based on the data from Spotify's Web API and
apps internal database.


There will be three roles: Guests, Listeners and Moderators.
Listeners can review albums, track listening progress, and create public
or private lists like "Top Jazz" or "My favorite albums" that could be added to their Spotify account if the user wishes.

Moderators can edit or remove inappropriate content, approve user-submitted
albums, feature top lists or reviews on the homepage and manage the music database.

Guests can browse public content, but only registered users can create lists,
review, and track their progress.

Listeners can search a database of albums and tracks (spotify or user-submitted),
and add them to personal libraries with statuses such as "listening,"
"completed," "dropped," or "wishlist."
Listeners can choose if their info should be automatically updated based on
Spotify activity.
Listeners are able to:
- Control currently played songs and queue
- Add albums or individual tracks to a personal library
- Update playtime and listening status
- Write reviews and rate albums
- Create and share themed playlists/lists
	Playlists can be collaborative(multiple users are managers)
- View community stats like:
	“Most listened genres this month” or “Longest albums completed”
- Compare total listening time by month or genre in personal analytics

Listeners will have a personal dashboard showing:
- Currently playing song
- Albums currently listening to
- Listening streak (e.g. days with music logged)
- Total time listened
- Favorite genres and artists (based on interaction)

Each album/single will display metadata
including artist, genre, release date, tracklist, and total playtime.
Overall popularity score and the amount of likes