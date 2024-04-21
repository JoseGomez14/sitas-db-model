# ER Model - SITAS - Universidad de Antioquia

> [!NOTE]  
> To add the script for your module, remember to read the contribution manual: [CONTRIBUTING.md](./CONTRIBUTING.md)

> [!IMPORTANT]  
> Remember to consistently use the same SQL formatter. It's available here: [Prettier SQL](https://marketplace.visualstudio.com/items?itemName=inferrinizzard.prettier-sql-vscode)

## Table descriptions

### ✈ Flight

Stores information about flights, including their unique identifiers, flight numbers, base prices, tax percentages, and surcharges.

### 🛫 AirplaneModel

Contains details about airplane models, such as their identifiers, families or types, passenger capacities, and cargo capacities.

### 🏬 Airport

Maintains data related to airports, including their unique codes, names, types (e.g., international, domestic), cities, countries, and the number of runways available.

### 📊 Scale

Manages the scales or segments of flights, recording details like unique identifiers, references to flight and airplane model, origin and destination airports, departure and arrival dates, and the price for each scale.

### 👨‍✈ Employee

Stores information about employees, including their unique identifiers, names, and job titles or positions within the airline company.

### 🚀 FlightCrew

Manages the flight crew members, recording details such as unique identifiers, references to flights and employees, and the roles or positions of crew members during flights.

### 👤 Passenger

Stores main info about passenger and the associated seat.

### 📄 Booking

Stores crucial information about the booking, such as the associated passenger, the booked flight, the booking date, the booking status and the total price.

### :package: Luggage

Manages each passenger's luggage and its unique characteristics, streamlining the process of identifying the appropriate zone for placement. Additionally, it enforces a strict limit on luggage allowance, with any excess baggage incurring an additional charge.

### :card_file_box: PlacementArea

Categorizes items based on their designated placement zone, which may include hand luggage, cabin luggage, or checked luggage.

### 🧳 LostLuggageInfo

Contains information about where to send luggage in case of lossing it.

### 💉 MedicalInfo

Stores info about passenger medical info

### 📨 Boardingpass

Gatters a lot of information from diferents moduls to generates a boarding pass


### 💳 PaymentMethod

Has the information about the different Payment Methods a user can use to pay a booking

### PaymentMethodXUser

Saves the information about what Payment Method was used by the user who payed a Booking

### 📇 IdentificationType
This table stores various types of identification along with their unique identifiers.

### 👤 Person
Stores information about users including their personal details.

### 📋 Position
Stores information about different positions within the organization. Example: passenger, employee, etc.

### 🔑 Privilege
Stores information about different privileges or permissions.

### 🤝 PersonPosition
Associates users with their respective positions.

### 🔓 PositionPrivilege
Associates positions with their respective privileges.

### 🔍 Search_History 
shows the search history of a particular person

### 🪑💺 SeatStatus
Saves status of a seat. AVAILABLE or OCCUPIED

### 📍 SeatLocation
Store location type of a seat: WINDOW, CENTER, AISLE

### 🎫 SeatClass
Storre class type of a seat: TOURIST, FIRST_CLASS, EXECUTIVE

### 💺 Seat
Save Seat's basic information. References to SeatStatus, SeatLocation, SeatClass, and Flight. Stores seat's label as seat_label. 

### 👤💺 SeatPassenger
Auxiliar entity to build relationship between a Seat and a Passenger.