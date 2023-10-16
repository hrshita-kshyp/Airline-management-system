# Airline-management-system

# Airlines Reservation System
The Airlines Reservation System is a system for reserving airplane seats. This is a Reservation System implemented in C++ with MySQL. With this program, users can reserve seats, view user tickets, check flight schedules, display all passengers, add new flights with details, edit and delete records. Additionally, there is an option to track flight departures and arrivals.

# Class db_response
- This class contains connection of the database.
- mysql_init is the initializer of mysql_real_connect
- mysql_real_connect connects to the database. (MySql server should open while connecting) the if statement shows the successful or failed connection.

# Function main
- Here firstly the clear screen command then the title command and the color command.
- db_response::ConnectionFunction() is create the connection to the database.
### The program features
- Reserve Seat.
- User Ticket.
- Flights Schedule.
- Display Passenger.
- Flight Details.
- Add Flight.
- Edit Flight.
- Delete Flight.
- Flight Leave And Arrive.
- Back To Menu.

# Function ReserveSeat
- User can reserve seat for passenger.
- Some user details need to fill up then the data of the user stored in the database with “Insert” query.
- Finally success message ensures the data added in the database or the failed message show the error code.
- Now the Exit Code runs and ask the user for go to menu or Reserve seat again.

# Function UserTicket
- On start the function ask for a user name
- Only few words can find desired result of the user
- The “Select” query with “where” statement can find the result
- Finally if the result find by the program successfully it show the information of the user
- Now the Exit Core runs and ask the user want to go to menu search again.

# Function FlightSchedule
- Initially the “Select” SQL query get all the data from database.
- In flight schedule the flight no., arrival, leave and destination of the flight are shown in the console
- Lastly the Exit Code runs and ask the user for go to main menu.

# Function DisplayPassenger
- In the console all the passenger details are displayed
- Finally the Exit Code runs and ask the user to go to main menu or exit from program.

# Function FlightDetails
- In the flight detail there is a switch case to go to different options
Add Flight, Edit Flight, Delete Flight, Flight Leave And Arrive and Back to Menu
- These options are for manipulate the flight detail in C++ program

# Function AddNewFlight
- Here firstly the program get all the flight information from user
- Then the information insert into the database with “Insert” query
- If the operation successfully done then the program shows the Success message or found any error then the program show error message with error code
- Finally the Exit Code runs and ask the user to go to main menu, insert again or exit from C++ program

# Function EditFlight
- Firstly the program shows all the flights in the database
- Then ask for a flight id from the user
- After verification of the given id the program see the id is in the database or not if not then shows not found message
- If the ID found by the program then it shows the row of the corresponding id and ask for change the values that the user want if the user don’t want to change any value then they can simply type ”X”.
- Now the “Update” query runs and if no exception found the console shows the success message
- Now the Exit Code runs and ask for the user to choose go to menu, edit another item or exit from the C++ program.

# Function DeleteFlight
- Firstly the program shows all the flights are stored in the database
- Then ask for an Column ID
- If the ID verification successfully done then it will check the id is in the database or not
- Or if the id verification is not successful then it runs the Exit Code
- If the id found successfully then the “Delete” query delete the data from the database
- Finally the Exit Code runs.

# Function FlightLeaveArrive
- Firstly some important flight information are displayed in the console
- Then ask for an Column ID
- If the ID verification successfully done then it will check the id is in the database or not Or if the id verification is not successful then it runs the Exit Code
- Now if the id found then the program show the details of the flight and some inputs “Leave, Arrive, Available” are ask for edit by the user.
- Finally the Exit Code runs.
