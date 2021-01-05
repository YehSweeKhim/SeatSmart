# SeatSmart
50.001 Introduction to Information Systems &amp; Programming: 1D Project

## Introduction
SeatSmart attempts to to solve three key library associated problems:
* Library goers wasting time having to find seats physically
* Library users hogging seats with their items
* Librarians having a difficult time monitoring all the seats efficiently, and unsure if they should clear the items to make space for other users

Head over to our [final report](/Final%20Report.pdf) to read more about SeatSmart and its system design and implementation.

## Solution
![Solution](/Images/solution.png)

### Scenario 1: 
The user’s presence will cause the seat status to be ‘Unavailable’, regardless whether any item is placed on the table.

### Scenario 2:
After a grace period of 20 minutes, if the items are still left unattended, the librarian will be alerted via a sound notification and an update on the right panel.

### Scenario 3: 
The seat status will become ‘Available’ if the librarian has cleared the item at that particular seat or if the user has left the seat with all his belongings

### Data Retrieval:
To retrieve data from the sensors into the Firebase, we created a python script that reads the serial output from the arduino IDE which will then be uploaded onto the Firebase. This is a stop-gap measure as we were unable to get the Arduino Wifi Module to work.


## SeatSmart Features
### Login Page
* Simple login page for the librarians (Only librarians have access to the email and password)

![Login Page](/Images/login_page.png)

### Main Page (Level 1 of the library)
* Seat status within the library
* Inform librarians on seats to be cleared (After a grace period of 20 minutes, if the items are still left unattended.) 

![Main Page](/Images/level1.png)

### Notes
* Allow librarians to take down notes or pass on information to the librarian on the next shift

![Notes Page](/Images/notes.png)

### Statistics
* Occupancy rate of the library

![Status Page](/Images/seat_statistics.png)

