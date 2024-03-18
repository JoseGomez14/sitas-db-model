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

### 📄 Reservation
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
