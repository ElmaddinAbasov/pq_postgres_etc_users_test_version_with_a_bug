# Working with PostgreSQL using C language and pq library.
## Program description

Looking for a better and more convinent ways to study information from a /etc/passwd file. So we decieded to write a relly small program that reads info from /etc/passwd file, parses its content and fill a small table in out database. Table store basically information about a user in Linux system.

We have couple modules in our system :

  - init modules initializes our system. We connect to a one of default databases that PostgreSQL provides us. Then we create a new database(etc_users), we close previous connection and then we establish a new connection with earlier created database.

  - parse module parses info from etc/passwd file and fills a structure with user_info array.

  - postgres_db modules just writes all info from a user_info to a table.


# For now program has one bug, and it terminated unsuccessfully because of it.

