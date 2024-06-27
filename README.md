# Olympic Data Management

## Introduction
The Olympic Data Management system captures the essence of the Olympic Games over the years. It stores data about host cities, participating countries, sports activities, and athletes who have participated in various tournaments.

## Purpose
The primary purpose of this database is to provide a structured and efficient platform for managing, organizing, and analyzing data related to the Olympic Games. It enables seamless retrieval of information crucial for stakeholders, organizers, and enthusiasts alike.

## Users
- Olympic organizers
- Athletes
- Sports enthusiasts
- Researchers

## Applications
- Effective planning and scheduling of Olympic activities
- Analyzing athlete performance for improvements
- Engaging fans with athlete profiles and real-time information
- Sending real-time event notifications and updates to athletes, coaches, and officials
- Forecasting future match statistics based on previous data

## Database Requirements
### Strong Entities
- **Olympic Occurrences**: Represents each Olympic occurrence.
- **Athlete**: Information about athletes who have participated in the Olympics.
- **Countries**: Details of countries that participated in at least one Olympic occurrence.
- **Tournaments**: Specific events within the Olympic Games.
- **Sports**: List of sports in the Olympics.

### Weak Entities
- **Coach**: Information about coaches.
- **Medals**: Design of medals used in each Olympic occurrence.
- **Torch**: Modern torches used in each Olympic occurrence.

### Relationship Types
- **Represents**: Relationship between Athlete and Country.
- **Rewards**: Relationship between Olympic Occurrences and Medal.
- **Organized_Under**: Relationship between Tournament and Olympic Occurrences.
- **Eternal_Flame_Of**: Relationship between Olympic Occurrences and Torch.
- **Trained_Under**: Relationship between Athlete and Coach.
- **Ranked_At_During**: Relationship between Countries and Olympic Occurrences.
- **Matches**: Relationship among Olympic Occurrences, Sports, and Tournaments.
- **Olympic_Arena**: Relationship among Olympic Occurrences, Countries, and Sports.
- **Athletic_Face_Off**: Relationship among Sports, Tournament, Countries, and Athlete.

### Functional Requirements
- **Insert**: Adding details of new athletes, tournaments, etc.
- **Update**: Modifying athlete information, tournament attributes, etc.
- **Delete**: Removing details of canceled tournaments, athletes not participating, etc.
- **Retrieval**: Searching and retrieving data based on specific criteria.

## Commands
### INSERT Command
- **Countries**: Insert a new country record into the table.
- **Athlete**: Add a new athlete to the database.

### DELETE Command
- **Countries**: Remove a country record from the database.
- **Athlete**: Delete an athlete from the database.

### UPDATE Command
- **Olympic Occurrence**: Modify host countries and winning countries.
- **Athlete**: Update information for a specific athlete.

### Selection - Projection
- **List of Countries**: Fetch a list of countries based on selected attributes.
- **List of Athletes**: Retrieve a list of athletes projected by age.
- **Torch**: Retrieve torches based on attributes.

### Search
- **Athletes by Name**: Find athletes based on a keyword in their names.
- **Sport by Name**: Locate a sport based on the initial keywords.

### Gender Distribution
- **By Sport**: Count of each gender participating in a sport.
- **By Athletes (All)**: Count the number of male and female athletes.

### Average Age
- **By Sport**: List the average age of athletes participating in each sport.
- **Of Athletes**: Calculate the average age of all athletes.

### Sum of Medals
- List of medals received for each country.

### Minimum Medals
- Identify athletes with the minimum medals received.

### Maximum Medals
- Identify athletes with the maximum total medals received.

### Get Country by Rank
- List countries based on rank thresholds.

### Country Participation
- List the countries and the number of seasons the country participated in.

## How to Operate
1. **Setting Up the Database**:
   - Ensure you have a database system installed (e.g., MySQL, PostgreSQL).
   - Import the database schema provided in the `schema.sql` file.

2. **Inserting Data**:
   - Use the provided `INSERT` commands to add new records.

3. **Updating Data**:
   - Utilize the `UPDATE` commands to modify existing records.

4. **Deleting Data**:
   - Use the `DELETE` commands to remove records from the database.

5. **Retrieving Data**:
   - Execute the `SELECT` queries to fetch specific information based on various criteria.

6. **Running Aggregations**:
   - Perform aggregate functions like `SUM`, `AVG` to analyze the data.

## Video Demonstration
For a detailed explanation of how the database works click the below link:
https://github.com/Vaishnavipriyaa/OlympicDataManagement/blob/main/OLYMPIC%20DATA%20MANAGEMENT/WorkingVideo.mp4
