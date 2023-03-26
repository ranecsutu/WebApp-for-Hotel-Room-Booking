# Bookings and Reservations

This is the repo for my bookings and reservations project.

- Built in Go version 1.18
- Uses [chi router](https://github.com/go-chi/chi)
- Uses [alex edwards SCS](https://github.com/alexedwards/scs/v2)
- Uses [nosurf](https://github.com/justinas/nosurf)

1. In the database.yml file enter your DB credentials.
2. Run "soda migrate" to generate tables in database. After this, manually add an user into the "users" table (use the hash of the password). You will need a user to authenticate on the Login page in order to view admin dashboard.
3. Run the program using CLI arguments like this: go run .\cmd\web\ -dbname 'DBNameHere' -dbuser 'DBUserHere' -dbpass 'UserPasswordHere'
