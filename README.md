# Group 7 Mist 4610 Group Project 1

## Team Name: 
Sp24_61608_Group 7

## Team Members:

1. Rohan Kothari [@Rohank66](https://github.com/Rohank66/MIST4610-GP-1.git)
2. Sedat Akgun [@sedatakgun](https://github.com/sedatakgun/MIST4610-GP-1.git)
3. Tharini R.K. [@tr64311](https://github.com/tr64311/MIST4610-GP-1.git)
4. Ruhi Shirke
5. Rachel Kim [@rachelkim816](https://github.com/rachelkim816/MIST4610-GP-1.git)
6. Danielle LaDuca [@danijlad](https://github.com/danijlad/MIST4610-GP-1.git)

## Problem Description:

As the owner of an esteemed soccer club, our primary mission is to conceptualize and implement a relational database tailored to the operations of a soccer club. Central to our model is the ‘Player’ entity, representing the athletes who form the core of the club’s ambitions and daily activities. This club operates through a series of interconnected components including team formations, coaching staff, match schedules, training sessions, and equipment management. Our goal is to meticulously model these relationships, populate the entities with carefully crafted sample data, and execute queries that yield actionable insights into the club’s functioning. By doing so, we aim to equip the management with the tools necessary for strategic decision making, ultimately ensuring the club's growth and success. 

## Data Model

Explanation of data model: 

Our model captures the operations of a soccer club, designed to manage everything from player development to match scheduling seamlessly. At the heart of our model lies the Players entity, which holds comprehensive data about each player, including personal details, contact information, and position. This entity is foundational because the players are the core of our club’s activities. 

Club serve as the backbone of our club, with each team composed of multiple players. This is represented by a one to many relationship between Club and Players, signifying that while a player belongs to a single team, a team comprises many players. Our players can be placed on one of three available teams, based on their skill level. The Club entity is linked to Coaches, reflecting the different roles coaches play in team strategy and player development. Each team is assigned 5 coaches, where they are responsible for guiding and managing their team’s progress. 

Further branching from the Players entity is PlayerStats, which documents the performance metrics of players, such as goals, assists, redcards, wins, and losses. This relationship explains the analytical aspect of our club where tracking individual performance is key to the overall team development. Players also connect to the Memberships entity, detailing whether or not their contract has been signed and the type of membership they opted for. 

Our club’s scheduling is captured through the MatchSchedule and PracticeBlocks entities. MatchSchedule determines the match dates and opponents, showing a one to many relationship between Club and MatchSchedule to account for the numerous matches a team engages in throughout the season. PracticeBlocks organizes practice sessions for players on certain days and times, showing a many to many relationship with Players and PracticeSchedule because players attend multiple practice sessions, and each session can accommodate multiple players. 

The EquipmentSets entity tracks the inventory of sports equipment indicating a many to one relationship with PracticeSchedule. This shows that while multiple practice sessions may use the same set of equipment, only one equipment set is used each practice. Each equipment set includes, quantity of pieces, purchase date, and the skill level associated with the kit.

Finally, facilities management is addressed through Facility, Fields, and GameStaff entities. Facility represents the club's physical infrastructure, linked to Fields to show the specific playing and practice areas within the facility. GameStaff is connected to Facilities through a one to many relationship, illustrating that the facility employs several staff members, while each staff member is associated with the one facility. Within GameStaff includes, first name, last name, and the job title for the staff. 


<img width="850" alt="Screenshot 2024-03-27 at 11 59 25 AM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/4c98178e-02a7-41af-9bf0-dc3cdec17465">



## Data Dictionary:

<img width="710" alt="Screenshot 2024-03-27 at 12 09 44 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/101defdd-2798-4b47-936a-9a8ebe19dc36">

<img width="694" alt="Screenshot 2024-03-27 at 12 46 38 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/39d6764e-223d-4b17-a1fc-fdbc29ae279a">

<img width="721" alt="Screenshot 2024-03-27 at 12 14 53 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/13284f5a-1c18-42e0-9f6b-9179cc9ee63e">

<img width="716" alt="Screenshot 2024-03-27 at 12 15 26 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/3b94ec26-faf2-4700-b9fc-48a3792ecb44">

<img width="696" alt="Screenshot 2024-03-27 at 12 15 39 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/2f82ac13-bc4a-404a-a0d9-d3113a99e242">

<img width="697" alt="Screenshot 2024-03-27 at 12 16 04 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/1bdd4187-4cb0-4bc9-88e8-aa9c55c2f07f">

<img width="695" alt="Screenshot 2024-03-27 at 12 16 30 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/488f0e74-ec9c-45db-bce9-e9193474c276">

<img width="714" alt="Screenshot 2024-03-27 at 12 16 53 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/67130668-3e99-4a09-a580-355fbadd21d2">

<img width="711" alt="Screenshot 2024-03-27 at 12 17 13 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/013e91ba-23d9-4345-b391-d515ae20fd42">

<img width="718" alt="Screenshot 2024-03-27 at 12 17 51 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/41c1a203-bb1e-40ed-acc2-045219d36313">

<img width="709" alt="Screenshot 2024-03-27 at 12 18 13 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/49f9f7f0-57f3-40f1-bc10-38442b0de8b1">

<img width="707" alt="Screenshot 2024-03-27 at 12 18 48 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/7a471d51-32b5-4903-a163-e2807a2004c0">


## Queries:

<img width="630" alt="Screenshot 2024-03-27 at 12 19 42 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/f7080312-98a9-45de-9ae4-376207430e6e">


1. Query 1 provides insights into the performance of different clubs based on the average number of goals scored by their players. The results are also ordered by the averageGoals scored. 

<img width="631" alt="Screenshot 2024-03-27 at 1 20 18 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/bef81343-380d-4c68-953c-f3111b5a8648">

Query 1 assists managers in assessing the goal-scoring performance of the 3 clubs. This will allow managers to easily discern which clubs demonstrate more power compared to others on the field. This data shows that club 2 may need more practice. Listing the results in descending order of average number of goals makes it easier to see which clubs need to prioritize their goal performance. A query of similar nature can be used to evaluate other performance statistics.  

2. Query 2 lists the number of game wins and game losses by each team level for players who have not received a red card. The data is listed in order of the team skill levels, beginner, intermediate, and advanced. 

<img width="635" alt="Screenshot 2024-03-27 at 1 21 47 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/5a1762ba-6a8b-4422-9dbf-20f3f489e6f3">

Query 2 enables managers to evaluate the overall performance of the participants who demonstrate sportsmanship across each team skill level, based on wins and losses. A manager could compare these outcomes to those wins and losses of players who have received redcards. Here, a manager would see that players who do not receive red cards do not have as many wins. A manager may conclude that beginners can afford to play more aggressively than advanced players who tend to have more wins with less redcards. 

3. Query 3 tells us the average salary per coach role. The average salaries are listed in descending order so we can immediately see who is being paid the highest. 

<img width="633" alt="Screenshot 2024-03-27 at 1 22 32 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/556cc2ae-1f7a-40d8-9f0b-bda9ae0bc37f">

Query 3 can be used in two ways. Firstly, it will prove our club is sufficiently paying each of our coaches. If not, this data may reveal to management a need to offer salary increases. Secondly, this data can be referenced during the hiring process. When managers send out offer letters to new coaches, they should offer a salary near this average. 

4. Query 4 lists the players with over 10 goals and complete contract status with “Platinum” membership.  

<img width="577" alt="Screenshot 2024-03-27 at 1 23 02 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/ff22a76f-37c4-46d0-9cfe-798d7e98c2a4">

Query 4 could be used by management to recognize and reward players who are high performing and fully engaged with the club. These are effectively our club’s “VIPs,” hence why the procedure is named valuePlayers(). This data will help managers of our club who wish to highlight the most successful players, recruit them for teams, or promote them at future events. 

5. Query 5 filters and lists players with first names starting from A to M who have practice times on ‘Grass’ fields. It utilizes REGEXP for pattern matching on names and joins to correlate practice schedule with field type. This allows for efficient allocation of training resources and plans.

<img width="624" alt="Screenshot 2024-03-27 at 1 23 53 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/8162c502-02f6-4eec-9d74-61ca9f66a625">

Query 5 shows the players with the first name beginning with A-M represent half of our players (named practiceBlock1 in the procedure) who will engage in their first practice activity (ex. shooting) on grass and then switch with the remaining players (N-Z) who were working on the other practice activity (ex. dribbling) on turf. A manager would reference this query to see when the first half of players are scheduled to practice on grass. The club can schedule appropriate practice sessions on grass fields for half the players, and turf fields for half the players optimizing field usage.

6. Query 6 provides detailed information about players with incomplete contract status and a loss history greater than 20.

<img width="626" alt="Screenshot 2024-03-27 at 1 24 24 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/8c71637c-b2d4-4873-9f26-aeaea487ce36">

Query 6 shows the players who have not resigned their contracts and have lost more than 20 games are listed. The club may want to review these players, specifically their incomplete contracts. Since the performance for these players reflects a high loss rate, managers may consider offering further training, a renewed contract, or strategy sessions. 

7. Query 7 lists the name, salary, job title, and zip code of game staff who reside in the same zip code as our facility, also known as our “local staff.”

<img width="594" alt="Screenshot 2024-03-27 at 1 26 23 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/e6d26ff6-42ae-4c68-8731-77d57c72c054">

Query 7 allows the club to know what staff members reside in the closest proximity to the facility. This is useful when there is a last minute cancellation of a referee or equipment manager and we need a staff member that can quickly commute to the location. 

8. Query 8 returns details of equipment sets that were purchased in 2022 and 2023 in a descending order. The details include equipment set level, quantity, purchase date and set ID.

<img width="632" alt="Screenshot 2024-03-27 at 1 27 22 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/533388e1-ab1e-41f9-9742-003be8438d31">

Query 8 is used when they wish to manage equipment history to make sure that the players have enough equipment that is up to date. This also allows the club to have access to view the equipment purchase history in relation to the equipment level, which can help them with future purchasing plans. Efficient equipment management ensures compliance with safety standards and regulatory requirements, mitigating risks of injury and liability for the club.

9. Query 9 lists out the matchScheduleIDs and the dates where there was not an opponent scheduled.

<img width="647" alt="Screenshot 2024-03-27 at 1 28 11 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/b601b0d1-59d5-417b-9e34-5bfb37b54807">

Query 9 allows the club to know which of its past matches have been canceled due to there not being an opponent available to play against. By knowing the day, month, and year, that the majority of cancellations occur, due to opponent unavailability, the club can better schedule their team’s matches in the future. This will set more accurate expectations for the players, parents, and coaches when planning their personal schedules.

10. Query 10 lists the first and last name of the head coaches whose salary is greater than the average head coach salary.

<img width="767" alt="Screenshot 2024-03-27 at 1 31 14 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/7415eab3-cf84-44b2-ab7a-d2d9f3d563b8">

Query 10 allows managers to see which head coaches are being paid more than average. This could create an uneven distribution of wages for reasons unknown. This higher than average salary can be further investigated to determine if these coaches’ time and dedication to the club equates to their above average pay and whether or not to adjust accordingly.

## Database information:

Name of the database: ns_Sp24_61608_Group7

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q1();
