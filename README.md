
# IMDB to JSON


Your can use this bash script to convert a IMDB movie info to JSON for [this](https://github.com/jsonmc/jsonmc) repository



## How to use

Every page in imdb has a **pageId** this script uses that pageId and pull the info from the page source. 

For exampel in this URL [https://www.imdb.com/title/tt0107290/](https://www.imdb.com/title/tt0468569/) pageId is **tt0107290**



```
$ git clone https://github.com/saderi/imdb-to-json
$ cd imdb-to-json
$ chmod +x imdb_to_json
$ ./imdb_to_json pageId_you_want
```  


### A movie has the following details


Movie attribute | Details
----------------|--------------
Release date | YYYY-MM-DD release date
Categories | Action, adventure, comedy, animation, family, fantasy, sci-fi
Director | Directors of the movie
Writers | Screenplay and story writers
Actors | Main casts of the movie
Year | Movie released year
Runtime | Runtime in mins
Storyline | Brief description of the movie


#### Example movie file

```json
{
  "name": "Jurassic Park",
  "year": 1993,
  "runtime": 127,
  "categories": [
    "adventure",
    "thriller",
    "sci-fi"
  ],
  "release-date": "1993-06-11",
  "director": "Steven Spielberg",
  "writer": [
    "Michael Crichton",
    "David Koepp"
  ],
  "actors": [
    "Sam Neill",
    "Laura Dern",
    "Jeff Goldblum"
  ],
  "storyline": "Huge advancements in scientific technology have enabled a mogul ... critical security systems are shut down and it now becomes a race for survival with dinosaurs roaming freely over the island."
}
```

