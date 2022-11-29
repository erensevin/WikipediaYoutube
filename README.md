# WikipediaYoutube
WikipediaYoutube is a python script written to automaticly download Wikipedia Articles and convert them into uploaded YouTube videoes. 
The application operates like this:
- Download a random wikipedia article with a specified length as an optional argument.
- Check if article already is generated and is valid
- Strip article of irrelevant content
- Split article up at linespaces for a max of 5000 bytes per piece
- Download relevant images from google for the title, with safe filter on to avoid NSFW content.
- Check for duplicate images and strips them if found
- Generate text-to-speech for each slice of the transcript
- Concatenate audio and images into one mp4 file. Also apply crossfade between images.
- Write the final mp4 and upload to Youtube using YouTube API v3

