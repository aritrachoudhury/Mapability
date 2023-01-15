# Mapability
A Geographic Information System for navigation

### Disclaimer ###
Posting the source code is stricly prohibited as istructed by the University of Toronto, Faculty of Applied Science and Engineering, since posting the source code from this project on a public website encourages plagiarism by future students, and reduces their learning by giving them a template for how to attack the project. Such public posting violates the copyright on the code provided to us by the teaching team and also places us at risk of being drawn into an academic integrity violation if a future student copies our work.

## Objective
Designed and developed a mapping software using C++ using the OpeStreetMap database. Concatinating the terms _Map_ + _Accessibility_ gave us the inspiration to create _Mapability_, a mapping software accessible for everyone and every need. 

## Milestones
The following milestones were successfully achieved by the team to successfully implment Mapability:
1. Using and Creating Efficient APIs
- Created new API functions from a library called libstreetdatabase that allows us to query geographic information database files for multiple cities
- Used STL data structures such as vectors and maps, and chose appropriate data strcutures to speed up an API
- Used unit tests to test our code

2. Visualizing an Interactive Map
- Visualized data, in this case a graph of a city map, using the EZGL graphics library
- Developed an user interface to respond to user queries and display data
- Used the gtk graphics library to use some of the more advance unser-interface functions

3. Shortes Path and Directions UI
- Implemented and optimized gshortest path search algorithms, namely:
  * Breadth First Search (BFS)
  * Depth First Search (DFS)
  * Dijkstra's Algorithm 
  * A* Algorithm
 - Used the EZGL graphics library to display a path between two intersectins through a search command

4. The Travelling Courier Problem (an optimized delivery system similar to the travelling salesman problem)
- Finding a valid path through a graph that passes through a set of vertices
- The following heuristical algorithms were developed to solve the problem:
  * Multi Dijkstra Method
  * Greedy Method
  * 2-opt
  - Ant Colony Method
  
## How to Use Mapability
Te dialog box provides all the functionalities required to ergonomically use the map:
- Panning features
- Directions from one point to another
- Landmarks such as hospitals, restaurants, parks, etc
- Computing path for the travelling courier
- Colour scheme according to users choice (Dark and Light mode, including accessiblity features for colour blindness)
![Screenshot 2023-01-14 at 2 21 41 PM](https://user-images.githubusercontent.com/97995705/212492650-d040cb87-80b1-4fba-a382-5b4a8d6f38d9.png)

Figure: Panning feature (Zooming in, zooming out)
![Screenshot 2023-01-14 at 2 20 34 PM](https://user-images.githubusercontent.com/97995705/212492664-efe62744-2f29-48d3-ae42-f9e3c1f45db1.png)

Figure: Directions between two points of interest

![Screenshot 2023-01-14 at 2 28 33 PM](https://user-images.githubusercontent.com/97995705/212492737-6cbbae43-9667-4297-9c49-dd981908b38c.png)

Figure: Dark mode and normal mode colour scheme

![Screenshot 2023-01-14 at 2 29 36 PM](https://user-images.githubusercontent.com/97995705/212492898-0587e788-4271-4975-b237-6b68b3515b93.png)
![Screenshot 2023-01-14 at 2 29 52 PM](https://user-images.githubusercontent.com/97995705/212492881-93cbd0d8-2eaf-480f-a25e-91f157a0230b.png)

Figure: Colour scheme options


The map also provides keyboard control for a mouse free experience as well as an About dialog box to seamlessly use all the features:

![Screenshot 2023-01-14 at 2 35 22 PM](https://user-images.githubusercontent.com/97995705/212492985-ea7f1edb-b43b-470f-a513-f8b37e38aaf9.png)

![Screenshot 2023-01-14 at 2 35 07 PM](https://user-images.githubusercontent.com/97995705/212492988-45fc4056-a7f1-46d4-92b2-7c3df962bdb6.png)

Lastly, leveraging Dijkstra's algorithm coupled with priority queue to store the best travel times, we were able to find the shortest and fastest path between two points of interest

![Screenshot 2023-01-14 at 2 38 29 PM](https://user-images.githubusercontent.com/97995705/212493255-4b6dd565-0b3c-4b06-a3ed-7753c38d6348.png)


