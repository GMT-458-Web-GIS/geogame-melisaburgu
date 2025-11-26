[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/BhShQpq1)



🚕 GMT 458 - GeoGame: NYC Geo-Predictor: Taxi Challenge

🗓️ Design Of the GeoGame

This document outlines the design, layout, and mechanics for the GeoGame project. The game is an interactive, time-based web application focused on geovisualization.



1. Project Requirements
   
The core functional requirements for the GeoGame are:

•	Geo-Component: The game will utilize NYC taxi data. This data should be pre-processed to reflect hourly and daily density patterns (e.g., rush hour).

•	Temporal Component: The game is time-based. The user must complete as many tasks as possible within a 60-second time limit.

•	Interaction: The user interacts with the browser by clicking on a map interface to identify geographic zones based on data visualization.

•	Advanced Visualization: The project will use an advanced visualization library to handle and display the large taxi dataset effectively.



2. Frontend Layout
   
The layout is designed to be intuitive, prioritizing the map interface.

<img width="599" height="461" alt="Ekran görüntüsü 2025-11-16 215826" src="https://github.com/user-attachments/assets/93baf992-fd89-468e-8bd8-e89f128d50b1" />

![WhatsApp Image 2025-11-16 at 22 00 20](https://github.com/user-attachments/assets/a3dcfb45-b3aa-4c9d-87b6-aa8c5bf9400c)



3. Game Mechanics
   
	How will the game progress (difficulty level, time-based progression)? 

•	Progression: The game is based on a 1-minute time limit to complete as many tasks as possible. When a user correctly answers, the visualization updates to the next task (e.g., the next hour or a different day).

•	Difficulty: Difficulty will increase dynamically. The game may start by asking for predictions in large boroughs and progress to asking for specific, smaller Taxi Zones.

•	Scoring: Correct answers yield points. Incorrect answers will apply a penalty based on the geographic distance from the click to the correct zone.


	How many questions will there be? 

•	The number of questions is not fixed. The objective is to correctly answer the maximum number of tasks within the 60-second time limit.


	How many lives, if any, does a user have? 

•	There will be no lives. The only constraint is time. Incorrect answers will result in a score penalty and consume valuable time.



4. Stated JavaScript Library
   
•	Main Library: Deck.gl (Advanced Geovisualisation and Data Analysis)

•	Reason: Leaflet and OpenLayers are options, but Deck.gl is chosen for its superior performance in handling large-scale datasets, specifically using its GridLayer and HeatmapLayer capabilities. 



🎮 Gameplay Mechanics & Instructions

1.	**Start the Game:** Click the **"START GAME"** button on the overlay screen to begin the simulation.

2.	**Objective:** Analyze the map and click on the **Red/Orange/Yellow zones** representing high taxi density areas to score points.

3.	**Day Cycle Progression:** As you score points, the game advances through realistic traffic scenarios: **Morning Rush -> Lunch Break -> Evening Rush**.

4.	**Infinite Loop (Day 2+):** The game simulates a continuous timeline. After completing the Evening session, it loops to **Day 2, Day 3, and beyond** with evolving challenges.

5.	**Game Over State:** You have a fixed time limit (60s). When the timer hits zero, a **"GAME OVER"** screen appears displaying your **Total Score** and a button to try again.

6.	**UI Controls:** Use the toggle button in the top-left corner to switch between **Dark Mode** and **Light Mode** map themes for better visibility.



🚀 Play Live Demo

Click Here to Play “NYC Geo-Predictor: Taxi Challenge”  : 

https://gmt-458-web-gis.github.io/geogame-melisaburgu/



