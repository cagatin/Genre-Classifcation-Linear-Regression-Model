# Genre Classification Machine Learning Model
Welcome to my genre classification model! The following file utilizes **nearest k neighbor classification** in order to predict whether a song is
hip-hop or country, using only the numbers of times words appear in the song’s lyrics.

## The Dataset
The dataset is a table of songs, each with a name, an artist, and a genre. 
<br>
The predict a song’s genre, we have some attributes: the lyrics of the song, in a certain format.
<br>
We have a list of approximately 5,000 words that might occur in a song. For each song, our dataset tells us how frequently each of these words occur in that song.
<br>
The dataset doesn’t contain all information about a song. For example, it doesn’t include the
total number of words in each song, or information about the order of words in the song, let
alone the melody, instruments, or rhythm.
<br>
<br>
This dataset was extracted from the Million Song Dataset
(http://labrosa.ee.columbia.edu/millionsong/). Specifically, we are using the complementary datasets from musiXmatch (http://labrosa.ee.columbia.edu/millionsong/musixmatch) and
Last.fm (http://labrosa.ee.columbia.edu/millionsong/lastfm).
<br>
<br>
The counts of common words in the lyrics for all of these songs are provided by the musiXmatch dataset (called a bag-of-words format). Only the top 5000 most common words are represented. For each song, we divided the number of occurrences of each word by the total number of
word occurrences in the lyrics of that song.
<br>
<br>
The Last.fm dataset contains multiple tags for each song in the Million Song Dataset. Some
of the tags are genre-related, such as “pop”, “rock”, “classic”, etc. To obtain our dataset, we first
extracted songs with Last.fm tags that included the words “country”, or “hip” and “hop”. 
<br>
<br>
These songs were then cross-referenced with the musiXmatch dataset, and only songs with musixMatch
lyrics were placed into our dataset. 
<br>
<br>
Finally, inappropriate words and songs with naughty titles
were removed, leaving us with 4976 words in the vocabulary and 1726 songs.
