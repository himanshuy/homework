# homework

###Postgres 
#####Start postgres on mac osx
`postgres -D /usr/local/var/postgres`
#####Create User
`createuser --pwprompt adminbhai`

`createuser admin` (without password)

#####Create a database
`createdb -Oadminbhai -Eutf8 mydb` (if db is not created)

#####Access the database

`psql -U adminbhai -W <mydb>`

######Quit
`\q`
