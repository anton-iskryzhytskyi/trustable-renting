# trustable-renting
The system to improve the renting experience, make it faster and easier for both tenant ad landlord

# Draft

## Functions
Interface is implemented as CLI
The system provides an application that allows for users
* Signup
* Login
* Check own renting records
* Open account info for specific user (for specific period of time)
* Request one time code exchange to add a renting records for specific user by current user and vice-versa 
  (in case of exchange accepted both current and specific user will add records to each other)
* Check a list of open accounts for current user
* Check a specific account open for current user
* Check a list of available requests of codes exchanges to add a renting records to another account for current user
* Accept request of codes exchange to add a renting records  
* Add a renting record to another account

## Entities
* User account - short person info (name, passport code, etc) plus renting records
* Request of one time code exchange - short exchange info (from user, when requested)
* Renting record - info about renting experience

## Code structure
* domain - domain entities and domain services
* business - application services and external services
* shared - could be used from anywhere and not influence on code logic - configs and logger
