# homework

###Postgres 

#####Install on ubuntu
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'

wget -q https://www.postgresql.org/media/keys/ACCC4CF8.asc -O - | sudo apt-key add -

sudo apt-get update

sudo apt-get install postgresql postgresql-contrib

sudo postgresql-setup initdb

//Configuration
sudo vi /var/lib/pgsql9/data/pg_hba.conf

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
