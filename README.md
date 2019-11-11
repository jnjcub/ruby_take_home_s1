#Problem 
  Write a ruby program to read from given data sources into a destination sink. Effort expected is not more than 1-2 hrs

  The sink is movie.json. The contents of the file is of the format

```json
  { 
    "movies" :  [ 
       { "m_id": "05dce573-9a96-4917-8263-f59b8e410cc2", "title": "Title one" },
       { "m_id": "0dce5731-9a96-4917-8263-f59b8e410cc2", "title": "Title ten" },
       ...
       { "m_id": "05dce732-9a96-4917-8263-f59b8e410cc2", "title": "Title Atwo" }
    ]
  }
```
  There are 3 source files. All of them are in csv format. The m_id in movies.json is mapped to MID in the csv.
  * The 'cast.csv' has a list names attached to a MID.
  * The 'score.csv' has a score attached to a MID.
  * The 'showdate.csv' has a show date attached to a MID.

  #TODO Read all the source files and enrich the movie.json file.

  The expected structure of the enriched movie.json would look something like the following:
 
```json
  {
    "movies" :  [
       { 
         "m_id": "05dce573-9a96-4917-8263-f59b8e410cc2",
         "title": "Title one", 
         "score" : 0.23331,
         "show_date": "2018-01-22",
         "cast" : ["Jim A", "Tim O", "O Jane"] 
       },
       { "m_id": "0dce5731-9a96-4917-8263-f59b8e410cc2", "title": "Title three" },
       ...
       { "m_id": "05dce732-9a96-4917-8263-f59b8e410cc2", "title": "Title seven" }
    ]
  }
  ```

