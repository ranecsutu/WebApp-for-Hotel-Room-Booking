# Bookings and Reservations

This is the repo for my bookings and reservations project.

- Built in Go version 1.18
- Uses [chi router](https://github.com/go-chi/chi)
- Uses [alex edwards SCS](https://github.com/alexedwards/scs/v2)
- Uses [nosurf](https://github.com/justinas/nosurf)

1. In the database.yml file enter your DB credentials.
2. In main.go update "driver.ConnectSQL = ..." line with these credentials.
2. Run "soda migrate" to generate tables in database.
3. 
 Alternative 1: To have access to the admin dashbaord page, first you need to manually register a user in the DB (password field needs to be the hash). Using email and password you can not login and access the admin dashbaord.
 Alternative 2: You can bypass step 3 by going into the routes.go file and commenting mux.Use(Auth) line. In this case you can just go to localhost/admin/dashbaord URL and you land directly on the admin dashboard page without the need to authenticate.
