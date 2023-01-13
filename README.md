# Path Planning for Multiple Agents
This script is a Python function that calculates the paths for multiple agents to cover an area of interest depending on their estimated remaining flight time. The function takes in the following inputs:

- drone_ids: a list of names/ids for the agents
- lowerLeft: x,y coordinates of the lower left corner of the area of interest
- upperLeft: x,y coordinates of the upper left corner of the area of interest
- lowerRight: x,y coordinates of the lower right corner of the area of interest
- upperRight: x,y coordinates of the upper right corner of the area of interest
- batteries: a list with the remaining flight time of each agent (in seconds)
- currentPositions: a list of each agent's current position (x,y coordinates)
- currentAlts: a list of each agent's current altitude (z in meters)
- xRange: the amount of divisions the algorithm will make in the x axis (default=10)
- yRange: the amount of divisions the algorithm will make in the y axis (default=10)t must maintain from each other (default: 0)

The function returns a dictionary, where each inner list represents the path for ech agent to cover the area of interest.

## Requirements
- Python 3.x
- math library
- geopy library

## Limitations
- The script assumes that the agents can fly at a constant speed and do not encounter any obstacles.
- The script does not take into account any external factors such as wind or weather conditions.
- The script does not guarantee optimal paths for the agents and may not be suitable for real-world applications.

## Author
[Andreas Anastasiou](https://github.com/aanast01)

## Contact
For any questions or feedback, please contact me via email: aanast01@ucy.ac.cy
