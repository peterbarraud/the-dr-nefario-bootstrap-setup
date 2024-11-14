# The Dr. Nefario setup
(Why?. Because I love that scene in `Despicable me` where `Dr. Nefario` packs all his stuff in one little suitcase and leaves)

1. Clone this repo
1. Start mariadb with: `db.start.bat`
1. Sign into mariadb with: `login.root.bat`
1. Create a database using `create database test`
1. Create a table using `test.sql`
1. Start the php server using: `php.start.bat`
1. Install the npm dependencies using `npm i`
1. Start your website with `npm start`
1. ~To use this as your website setup, you'll need to .gitignore the mariadb and php dirs from the backoffice folder

## Backoffice
### Object layer
We have this PHP-based object layer to keep things as simple as possible. It's not very complicated, but seems to work pretty well.

(**Note** We still haven't accounted for many-to-many relations)
#### Creating an object
So, let's say you have an entity like user (let's call this `app user`). Which means you need an app user 
