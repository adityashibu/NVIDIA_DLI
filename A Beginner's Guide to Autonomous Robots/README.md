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

