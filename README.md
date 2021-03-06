# virtualMM

Plan:

1) Fetch CR transcripts from both campaigns.
2) Separate data to Players and DM - input and output
3) Use GPT-3 language model / ML to train an agent from the Matt Mercer's responses.

## So far

* **get_video_ids.py**: uses google api to fetch the video id of each video in a playlist. Only works for max 50 elements 
for some reason.

* **get_transcript_data.py**: downloads the transcripts from a list of youtube video ids (last part of the url) 
and saves them to a JSON file.

* **file_utils.py**: saving data to files and loading data from files.

* **read_transcripts.py: ** reads the json data and finds speaker and dialogue text units. Filters out players and dms.

## todos

* organize / restructure transcript data. How much does time axis matter? Include intervals?
* interpret words / contextualize them - add some kind of language model
* which ML method / architecture to use? train a NN to get a response word cloud and build response using a language model.

## Resources

https://github.com/roddds/critrole/blob/master/criticalrole%20talking.ipynb