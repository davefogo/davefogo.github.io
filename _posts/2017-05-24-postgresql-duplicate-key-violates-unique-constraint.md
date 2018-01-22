I have been refactoring my bookmark application Davemarks to get it working to my liking. Yesterday I uploaded about 1000 bookmarks compiled in CSV format from various sources. When I tried to add new ones after the import I couldn’t save new ones. I kept getting “duplicate key violates unique constraint” which means the database is trying to save records with keys (id) that had already been used. i.e (I was going to save a new entry to id 1, in reality it had to use id 1025). This happens when your database get out of sync.

Large imports (we can call 1000 rows large) commonly cause this bug. I looked online and found these links article & stackoverflow that helped me solve the issue.

This is what I did:

1. Log into the heroku pg database on terminal (mac)

```
heroku pg:psql
```

2. Check what my highest used id value for my table (bookmarks) was (using SQL)

```
SELECT MAX(id) FROM bookmarks;
# returned 1025
```

3. Check what my next id is

```
SELECT nextval('bookmarks_id_seq');
# returned 1
```

4. Obviously there is no synchrony here 1025 > 1. So, I set my highest used id as the starting point to add the next id (starting point 1025 -> next id for use is 1026).

```
SELECT setval('bookmarks_id_seq', (SELECT MAX(id) FROM bookmarks));
```
