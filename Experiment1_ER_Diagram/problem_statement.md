# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
<img width="1280" height="808" alt="image" src="https://github.com/user-attachments/assets/5052fa10-48ac-4fba-a755-da7804f0ab11" />


### Entities and Attributes
<img width="1077" height="369" alt="image" src="https://github.com/user-attachments/assets/aba60714-7e6b-4b16-8a19-6cb3efa54701" />


### Relationships and Constraints

<img width="1082" height="510" alt="image" src="https://github.com/user-attachments/assets/799e3851-a792-422b-bd3e-813c7db10677" />


### Assumptions
```
1.Each member must have at least one active membership.
2.A program may have multiple trainers, but at least one is mandatory.
3.Members can attend multiple sessions; attendance is recorded separately.
4.Personal training sessions are modeled as “Session” with specific trainer and member.
5.Payments can be for either membership fees or personal sessions
```
# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
<img width="1066" height="549" alt="image" src="https://github.com/user-attachments/assets/c70e8daf-dd8b-46cd-ab71-72a71d8ed4a1" />


### Entities and Attributes

<img width="1083" height="476" alt="image" src="https://github.com/user-attachments/assets/8d7c386a-807b-446d-9783-fa717b0c16ac" />

### Relationships and Constraints

<img width="1075" height="446" alt="image" src="https://github.com/user-attachments/assets/13569170-994e-41e4-8674-d194cc4d659a" />

### Assumptions
```
1.A member must exist before borrowing a book or registering for an event.
2.A book can only be borrowed by one member at a time.
3.Every event must be hosted in exactly one room.
4.Events may have zero or multiple speakers.
5.Overdue fines are calculated and stored in Loan.
```
# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
<img width="1067" height="676" alt="image" src="https://github.com/user-attachments/assets/f1acbb65-8ea3-4d3f-a94e-c07353db344e" />


### Entities and Attributes
<img width="1282" height="603" alt="image" src="https://github.com/user-attachments/assets/fd00b55c-b7c1-4544-b52a-cd55fb0e4d45" />

### Relationships and Constraints

<img width="1267" height="607" alt="image" src="https://github.com/user-attachments/assets/24148c69-c4e3-443c-acc1-eac20fc3309c" />


### Assumptions
```
1.A customer must exist before making a reservation.
2.Walk-in customers are treated as reservations with immediate booking.
3.Each reservation is linked to exactly one table.
4.An order can only be placed after a reservation exists.
5.One bill is generated per reservation (covers food + service).
6.A reservation can be served by one or more waiters.
```
### RESULT
Thus the ER Diagram for each scenario has been drawn and explained successfully.
