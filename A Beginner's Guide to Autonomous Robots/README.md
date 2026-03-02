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

Following are different types of sensors used for sensing along with their pros, and their uses.
| Camera Type | Pros | Uses |
| --- | --- | --- |
| **Monocular Cameras** (single-lens cameras that capture 2D images) | Simple, cost effective, widely available | Basic object detection, image recognition, simple navigation tasks |
| **Stereo Cameras** (two lenses capturing images simultaneously, mimicking human binocular vision) | Depth perception, 3D information | Obstacle avoidance, 3D mapping |
| **RGB-D Cameras** (RGB color imaging with depth sensing) | 2D color images with depth perception and 3D information | Advanced navigation, object manipulation and interaction |
| **Thermal Cameras** (create images based on temperature differences) | Effective in dark environments, effective through smoke or fog | Search and rescue missions, surveillance operations |
| **Event-Based Cameras** (capture brightness changes/events) | High temporal resolution and low latency | High-speed motion detection and tracking |
<br>


| LiDAR Type | Pros | Uses |
| --- | --- | --- |
| **2D LiDAR** (LiDAR that only shoot beams along 2D plane (X, Y)) | Simple, cheaper, and faster but limited functionality | Basic planar navigation and obstacle detection |
| **3D LiDAR** (LiDAR that shoots beams along a 3D plane (X, Y, Z)) | Detailed spatial information, wide field of view, and high resolution | Autonomous vehicle mapping |
| **Solid-State, Flash, and MEMS Lidar** (Laser pulses to measure distances) | Measure distances like other LiDARs and detailed maps | Autonomous vehicle mapping |
<br>


| Sensor Type | Pros | Uses |
| --- | --- | --- |
| **Ultrasonic Sensors** | Affordable and commonly used in low-cost robots | Distance measurement based on echo return time, home vacuum cleaners |
| **Radar** | Reliable in diverse conditions, provides distance, speed, and size information | Robotaxis |
| **GPS** | Essential for outdoor localization | Outdoor localization and navigation |
| **IMU (Inertial Measurement Unit)** | Measures acceleration and rotational rates to track motion and orientation, widely used in mobile robots | Motion tracking and orientation estimation |
| **Wheel Encoders** | Measure wheel rotation to determine travel distance | Odometry and distance tracking |
| **Magnetic Sensors (Compasses)** | Detect the Earth’s magnetic field to determine orientation and heading | Heading estimation and orientation reference |
| **Environmental Sensors** | Measure temperature, humidity, and air quality | Environmental monitoring |
| **Touch Sensors** | Cost-effective and useful for detecting contact, commonly used in household robots | Contact detection and collision sensing |


### Perception
Perception is crucial for enabling autonomous robots to understand their environment. Just as humans use a combination of senses like sight, hearing, and touch to interpret the world around them, robots rely on sensor fusion. This process integrates data from multiple sensors to create a detailed and accurate representation of the environment.

**Key components of perception:**
- **Sensor Fusion:** As the name suggests, Fusion of data from multiple different sensors to provide a detailed view of the surroundings.
- **Object Detection and Recognition:** Identifies and classifies different objects within the robot's environment.
- **Object Tracking:** Continuously track/follow an object as it moves, similar to how our eyes move to follow an object.
- **Scene Understanding:** Understand the overall context of what the robot is seeing so it can make informed decisions.


### Localization and Mapping
Localization and mapping are essential for robots to navigate and interact with their environment effectively. Imagine a robot as a traveler who needs a map and a compass to explore unfamiliar territory. These processes enable the robot to determine its position and create a map of its surroundings.

**Why Localization?**
Localization helps the robot identify its position within an environment. Without localization the robot would be a lost sailor at sea. In tasks like trajectory following or tracking, it is essential that the robot knows the exact position so it can follow the intended path accurately.
- **GPS (Global Positioning System):** Used outside (most of the time) to provide location data.
- **Visual Odometry:** Uses the camera to estimate movement, making it a computational task.
- **LiDAR based localization:** Matches the current position map with pre-existing map using LiDAR.

**Mapping Techniques:**
- **SLAM (Simultaneous Localization and Mapping):** A technique where robots both localize and map at the same time.
- **Occupancy Grid:** Represents the environment as grids with each cell indicating the probability of being occupied.
