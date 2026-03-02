# A Beginner's Guide to Autonomous Robots
This section contains notes for the topic "A Beginner's Guide to Autonomous Robots"

## Robotic Systems and Architectures
![System Architecture](images/sys_arch.png)
- **Perception and Localization:** Utilizes sensors such as cameras and LIDAR, along with mapping systems, to assess the environment and determine the robot’s position and state.

- **Planning:** Planning involves multiple stages.
    - **Global Planning:** Similar to setting a route on a map, defining the mission and waypoints to reach a goal.
    - **Behavior Planning:** Determines actions, such as which object to manipulate and how.
    - **Local Planning:** Generates trajectories for specific tasks, guiding the robot through precise paths.

- **Control and Actuation:** The controller tracks trajectory states to execute movements, whether for manipulation or navigation. Outcomes are tested in both virtual simulations and real-world scenarios.

- **Feedback Loop:** Continuously gathers data from sensors and localization to refine planning and improve system performance. This iterative process ensures adaptive and responsive robot behavior.

## Enabling Autonomous Robots
### Sensing
Sensing is crucial for enabling autonomous robots to understand their environment. This overview explores the different types of cameras and sensors used in robotics, highlighting their unique advantages and applications.

Following are different types of cameras used for sensing along with their pros, and their uses.
| Camera Type | Pros | Uses |
| --- | --- | --- |
| **Monocular Cameras** (single-lens cameras that capture 2D images) | Simple, cost effective, widely available | Basic object detection, image recognition, simple navigation tasks |
| **Stereo Cameras** (two lenses capturing images simultaneously, mimicking human binocular vision) | Depth perception, 3D information | Obstacle avoidance, 3D mapping |
| **RGB-D Cameras** (RGB color imaging with depth sensing) | 2D color images with depth perception and 3D information | Advanced navigation, object manipulation and interaction |
| **Thermal Cameras** (create images based on temperature differences) | Effective in dark environments, effective through smoke or fog | Search and rescue missions, surveillance operations |
| **Event-Based Cameras** (capture brightness changes/events) | High temporal resolution and low latency | High-speed motion detection and tracking |
