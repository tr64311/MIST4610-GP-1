# Group 7 Mist 4610 Group Project 1

## Team Name: 
Sp24_61608_Group 7

## Team Members:

1. Rohan Kothari [@Rohank66](https://github.com/Rohank66/MIST4610-GP-1.git)
2. Sedat Akgun 
3. Tharini R.K. 
4. Ruhi Shirke
5. Rachel Kim [@rachelkim816](https://github.com/rachelkim816/MIST-4610-group-project.git)
6. Danielle LaDuca [@danijlad](insert website)

## Problem Description:

As the owner of an esteemed soccer club, our primary mission is to conceptualize and implement a relational database tailored to the operations of a soccer club. Central to our model is the ‘Player’ entity, representing the athletes who form the core of the club’s ambitions and daily activities. This club operates through a series of interconnected components including team formations, coaching staff, match schedules, training sessions, and equipment management. Our goal is to meticulously model these relationships, populate the entities with carefully crafted sample data, and execute queries that yield actionable insights into the club’s functioning. By doing so, we aim to equip the management with the tools necessary for strategic decision making, ultimately ensuring the club's growth and success. 

## Data Model

Explanation of data model: 

Our model captures the operations of a soccer club, designed to manage everything from player development to match scheduling seamlessly. At the heart of our model lies the Players entity, which holds comprehensive data about each player, including personal details, contact information, and position. This entity is foundational because the players are the core of our club’s activities. 

Teams serve as the backbone of our club, with each team composed of multiple players. This is represented by a one to many relationship between Teams and Players, signifying that while a player belongs to a single team, a team comprises many players. Our players can be placed on one of three available teams, based on their skill level. The Teams entity is linked to Coaches, reflecting the different roles coaches play in team strategy and player development. Each team is assigned 5 coaches, where they are responsible for guiding and managing their team’s progress. Furthermore, there is a one to one relationship between Teams and Coaches indicating only one Head Coach to exist in each team. 

Further branching from the Players entity is PlayerStats, which documents the performance metrics of players, such as goals, assists, redcards, wins, and losses. This relationship explains the analytical aspect of our club where tracking individual performance is key to the overall team development. Players also connect to the Memberships entity, detailing whether or not their contract has been signed and the type of membership they opted for. 

Our club’s scheduling is captured through the MatchSchedule and PracticeBlocks entities. MatchSchedule determines the match dates and opponents, showing a one to many relationship between Teams and MatchSchedule to account for the numerous matches a team engages in throughout the season. PracticeBlocks organizes practice sessions for players on certain days and times, showing a many to many relationship with Players and PracticeSchedule because players attend multiple practice sessions, and each session can accommodate multiple players. 

The EquipmentSets entity tracks the inventory of sports equipment indicating a many to one relationship with PracticeSchedule. This shows that while multiple practice sessions may use the same set of equipment, only one equipment set is used each practice. Each equipment set includes, quantity of pieces, purchase date, and the skill level associated with the kit.

Finally, facilities management is addressed through Facility, Fields, and GameStaff entities. Facility represents the club's physical infrastructure, linked to Fields to show the specific playing and practice areas within the facility. GameStaff is connected to Facilities through a one to many relationship, illustrating that the facility employs several staff members, while each staff member is associated with the one facility. Within GameStaff includes, first name, last name, and the job title for the staff. 


<img width="850" alt="Screenshot 2024-03-27 at 11 59 25 AM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/4c98178e-02a7-41af-9bf0-dc3cdec17465">




## Data Dictionary:

<img width="710" alt="Screenshot 2024-03-27 at 12 09 44 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/101defdd-2798-4b47-936a-9a8ebe19dc36">

<img width="691" alt="Screenshot 2024-03-27 at 12 13 22 PM" src="https://github.com/Rohank66/MIST4610-GP-1/assets/104539792/53efcc85-8381-499d-b67f-23a1ff308f92">

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


1. Query 1 lists the number of reservations at each dining establishment that were made for between 6 and 8pm as well as the name of each dining establishment these reservation were made for. The results are also ordered by number of reservations in descending order.

![Screen Shot 2023-03-31 at 5 50 12 PM](https://user-images.githubusercontent.com/128402101/229239154-7637136b-5ddd-400c-9335-f3e571507ed7.png)

Query 1 allows allows managers to see which establishments have received the most number of reservations during their busiest time (6-8pm) which is typically dinner time. These establishments likely need more support, resources, and personnel around dinner time. Therefore, this query allows managers to identify which establishments to allocate this extra help to. Listing the results in descending order of number of reservations makes it easier to see which establishment to prioritize.

2. Query 2 lists the number of dining reservations made by guests on each floor. The results are ordered in ascending order of floor number.

![Screen Shot 2023-03-31 at 5 50 39 PM](https://user-images.githubusercontent.com/128402101/229239237-725cac35-598a-49e5-9b5d-bfc96fb18714.png)

Query 2 allows managers to see whether there is a trend between what floor a guest stays on and how much they reserve tabes at the resort's dining establishments. If managers were to find that dining reservations decreased as the floor number increased, it would have possibly indicated that guests were not dining at dining establishments because they felt the distance of the dining establishment from their room was too far and inconvenient.

3. Query 3 lists the information for all the guests who have not made an activity reservation.

![Screen Shot 2023-03-31 at 5 52 01 PM](https://user-images.githubusercontent.com/128402101/229239403-19acc956-7345-406e-b7ba-a6eaf1c8db88.png)

Query 3 allows the resort to market toward specific customers and contact them (e.g. promotional emails/coupons) about must-try activities. This helps to maximize revenue and increase efficiency by specifically targeting those who are not engaging in activities, rather than wasting time and resources to advertise to those who are already aware of and partaking in these activities.

4. Query 4 lists the names and phone numbers of dining employees who work in the highest rated dining establishment.
 
![Screen Shot 2023-03-31 at 5 53 30 PM](https://user-images.githubusercontent.com/128402101/229239730-7f5416bd-0aff-4c4a-b64d-7f365f246a36.png)

A restaurant with a high star rating is a large source of revenue for the resort and management may want to know the names of the employees who work there and how to contact them to reward them for maintaining such a high achieving restaurant (e.g. via a bonus, raise, awards, recognition) or to know which employees to target for continuous training and supervision in order to keep service within the establishment in top shape.

5. Query 5 lists the guests’ names and the hotel they are checking into if their reservation is during the PM, their room is a single or suite, their check in dates are between 2023-04-01 and 2023-04-10, and their hotel rating is above a 4.

![Screen Shot 2023-03-31 at 5 54 41 PM](https://user-images.githubusercontent.com/128402101/229239947-e3c0ab47-c77c-474b-81c1-1b187548b89c.png)

Query 5 allows the resort to manage how busy their check in will be during the PM hours of early April in their better hotels where the check in rooms are singles or suites. This can help the resort determine how many employees need to be working the check in desks to check in single or suite reservations in the afternoon of these dates in these specific hotels.

6. Query 6 lists the names of guests who have over 10 activity reservations and the activities that they have those reservations in.

![Screen Shot 2023-03-31 at 5 55 37 PM](https://user-images.githubusercontent.com/128402101/229240045-10ca60c7-1cb2-49e2-a224-256c841e5fd8.png)

Query 6 allows the resort to determine what guests are contributing the most to each activity’s revenue. The resort may use this information to reward guests who spend the most on activities by offering special prizes and promotions, creating guest loyalty and creating an incentive to reserve even more.

7. Query 7 lists the the amount of dining reservations per guest and the average amount of guests these reservations have.

![Screen Shot 2023-03-31 at 5 56 06 PM](https://user-images.githubusercontent.com/128402101/229240108-152740f1-4c85-4a38-9194-c981cf33fc42.png)

Query 7 allows the resort to see how many guests they should plan to seat, how the tables should be set up, and can lead to the resort figuring out how much revenue should be expected for the average visit.

8. Query 8 lists the guestID, guest name, and the number of room reservations per guest.

![Screen Shot 2023-03-31 at 6 34 05 PM](https://user-images.githubusercontent.com/128402101/229244470-c29f68b3-f837-4a18-97bb-f86345b84431.png)

Query 8 allows the resort to identify their frequent customers and how many times they have stayed. This could lead to a card system down the line. If a guest reaches 5 or 10 visits, there could be a platinum card which would gift the user reservation priority, food discounts, and other perks.

9. Query 9 lists all the rooms along with their average room view rating if the rating is above a 4 star. Additionally, the query is sorted by the view rating and arranged in descending order.

![Screen Shot 2023-03-31 at 5 56 31 PM](https://user-images.githubusercontent.com/128402101/229240166-bb0bc849-08dd-4521-8608-7a85ff53ae46.png)

Query 9 allows the employees and customers to see which rooms have an average view rating of 4 or more. Rooms with extravagant views are huge attractions to customers and can be a deciding factor when picking which room to stay in. This will help employees find which rooms have the best views fast and efficiently when asked.

10. Query 10 lists the names and prices of all activities offered by the resort that have not yet been booked by any guests and that are less than or equal to $50. Additionally, the results of the query are ordered by price in ascending order.

![Screen Shot 2023-03-31 at 5 57 00 PM](https://user-images.githubusercontent.com/128402101/229240218-c01fb32b-5f71-4562-b014-b656bfe051bb.png)

Query 10 allows the employees and customers to see what activities have not been booked yet, and the prices for these activities. The price is sorted in ascending order to make it easier to find the most affordable activities which most people are looking for. Activities are a huge part of the resort experience and using this script will make it easy for employees to find which activities are available as well as the prices for these activities.

## Database information:

Name of the database: ns_21479_1

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: 
CALL TP_Q1();
