#Problem 
  Write a ruby program to read from given data sources into a destination sink.
  Effort expected is not more than 2-3 hrs

```
  There are 4 source files. Three of them are in csv format and one in json.
  * The 'title.json' has a list names attached to a MID.
  * The 'cast.csv' has a list names attached to a MID.
  * The 'score.csv' has a score attached to a MID.
  * The 'showdate.csv' has a show date attached to a MID.

  #TODO Read all the source files and enrich the movies.json file.

  Send us the ruby program, the enriched movies.json and instructions to run the ruby program.
 
```json
  {
    "movies" :  [
       { 
         "mid": "05dce573-9a96-4917-8263-f59b8e410cc2",
         "title": "Title one", 
         "score" : 0.23331,
         "show_date": "2018-01-22",
         "cast" : ["Jim A", "Tim O", "O Jane"] 
       },
       { "mid": "0dce5731-9a96-4917-8263-f59b8e410cc2", "title": "Title three" },
       ...
       { "mid": "05dce732-9a96-4917-8263-f59b8e410cc2", "title": "Title seven" }
    ]
  }
```

