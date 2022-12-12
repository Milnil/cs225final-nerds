# CS225 Final Project: Airport Navigation Tool
### [Presentation Video](URL)
## Data
We will be using datasets from [OpenFlights](https://openflights.org/data.html). Specifically, we will be utilizing the airport dataset and route dataset in our project.
* [Airport Navigation Tool Nodes](https://raw.githubusercontent.com/jpatokal/openflights/master/data/airports.dat) (Airport ID, Location, Set of Neighbors)
* [Airport Naviation Tool Edges](https://raw.githubusercontent.com/jpatokal/openflights/master/data/routes.dat)

## Repo Structure
### Deliverables
* All major files that contain our functions and classes are in the [src](https://github.com/Milnil/cs225final-nerds/tree/main/src) directory.
* Datasets are stored as csv files in `/data`
* Tests are in `/tests`
* Project report, development log, contract, etc. are in `/documents`

## Running Instructions
Make sure you are running the program in Docker. If not, follow [this guide](https://courses.engr.illinois.edu/cs225/sp2022/resources/own-machine/) to get started.

### Executable
To use our Airport Navigation Tool, run the following in the root directory of the repository:
```
mkdir build
cd build
cmake ..
make
./main
```
Then follow the instructions in the terminal

We call all functions in main for you. The required inputs for each of the functionality are as follows:

* Flight Path Exists (BFS)
  * Input: two Integer IDs for the source airport and destination airport 
  * Output: a boolean that states whether a path from the starting and ending airport exists
* Shortest Path (Dijkstra's)
  * Input: two Integer IDs for the source airport and destination airport 
  * Output: the shortest path between the airport nodes represented as a vector of Integers
* Strongly Connected Components (Kosaraju's)
  * Input: an Integer ID for an airport
  * Output: a list of airport IDs that have a path to input airport

In addition to the above functions called in `/entry/main.cpp`, you can also refer to the input and output definitions in the comments for each small function in  `graph.h` and `/data`. 
### Tests
To run the test cases, run `make test` then `./test` in the root directory.

We constructed several small to medium sized datasets in `/data` directory.

 

## Team
*  Ayush Basu (` ayushb3 `)
*  Jessica Ho (` jmho3 `)
*  Milind Philar (` mphilar2 `)
*  Joy Wan (` joywan2 `)
