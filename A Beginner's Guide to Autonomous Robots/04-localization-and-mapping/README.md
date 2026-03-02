# Localization and Mapping

Localization and mapping are essential for robots to navigate and interact with their environment effectively. Imagine a robot as a traveler who needs a map and a compass to explore unfamiliar territory. These processes enable the robot to determine its position and create a map of its surroundings.

## Why Localization?

Localization helps the robot identify its position within an environment. Without localization the robot would be a lost sailor at sea. In tasks like trajectory following or tracking, it is essential that the robot knows the exact position so it can follow the intended path accurately.

### Localization Techniques

- **GPS (Global Positioning System):** Used outside (most of the time) to provide location data.
- **Visual Odometry:** Uses the camera to estimate movement, making it a computational task.
- **LiDAR based localization:** Matches the current position map with pre-existing map using LiDAR.

## Mapping Techniques

- **SLAM (Simultaneous Localization and Mapping):** A technique where robots both localize and map at the same time.
- **Occupancy Grid:** Represents the environment as grids with each cell indicating the probability of being occupied.
