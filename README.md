# Spotify Data Visualizer

**[This web application](https://spotify-streaming-visualizer.herokuapp.com/)** enables users to make use of their Spotify data.  With this app, users can upload their downloadable streaming data from Spotify &ndash; from there, the files are parsed and the user is presented with 2 responsive custom charts that detail their top 10 tracks and artists, along with the total play time for each (in minutes).

## Spotify Data Template

The file uploader expects a JSON file in the following format (default Spotify streaming data format):

```json
{
    [
        {
            "endTime" : "2019-08-01 00:02",
            "artistName" : "Artist",
            "trackName" : "Track",
            "msPlayed" : 224920
        },
        {
            "endTime" : "2019-08-01 00:06",
            "artistName" : "Artist",
            "trackName" : "Track",
            "msPlayed" : 224920
        },
        {
            "endTime" : "2019-08-01 00:09",
            "artistName" : "Artist",
            "trackName" : "Track",
            "msPlayed" : 224920
        }
    ]
}
```

![](https://i.ibb.co/mDNL9cW/data-visualizer-artists.png)

![](https://i.ibb.co/NCmdrZr/data-visualizer-tracks.png)

## The Stack
- NodeJS & Express &mdash; *Server*
- Vanilla HTML & JavaScript &mdash; *UI / UX*
- [Chart.js](https://www.chartjs.org/) &mdash; *Custom Charts*
- jQuery

## Deployment
- Heroku &mdash; the Data Visualizer web application is hosted on a free tier Heroku Dyno.  The NodeJS server currently hosts the static HTML file.