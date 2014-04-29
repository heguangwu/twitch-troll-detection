twitch-troll-detection
======================

Unsupervised machine learning methods to detect and classify anomalies in streaming data. We apply this to the viral event, TwitchPlaysPokemon, and attempt to identify trolls in a live IRC chat.

We use Java 7 and Python 3.4.0 in this repository. NumPy 1.8.1 and SciPy 1.8.1 were used in conjunction with Python 2.7.6.

We made the dataset we collected publicly available:
http://www.cs.utexas.edu/~ahaque/twitchplayspokemon.tar.gz (561 MB compressed, 3.4 GB uncompressed XML file)

mapreduce
--------
The Hadoop 2.2.0 program parses XML-like input we collected from the Twitch Plays Pokemon IRC chat room and groups all messages by user. This will allow us to build a profile for each user who participated.

python
--------
This project is the bulk of the unsupervised algorithm. It contains all necessary classes: Context, Message, User, etc. To import this project into eclipse, you must have PyDev installed.