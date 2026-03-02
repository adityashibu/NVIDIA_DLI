# Navigation and Path Planning

Navigation and Path Planning are important to ensure that robots can move efficiently and safely through their environments. This involves several layers of planning, each with a specific focus.

## Classical Navigation Systems

- **Routing and Mission Planning** uses algorithms such as A*, D*, and RRT (Rapidly-exploring Random Tree). This is similar to getting decisions at an intersection deciding whether to go left or right. Most of the time this along isn't enough so we bring in motion planning.

- **Motion planning** generates a sequence of movements for the robot to follow, allowing for a planned path along with obstacle avoidance. It usually takes a few seconds to process both the decision making and trajectory generation.
    - **Decision Making:** Focuses on behavior planning and interactions, such as deciding whether to navigate around obstacles like pallets or yield to moving forklifts.
    - **Trajectory Generation:** Involves creating a time-based trajectory, detailing speed, acceleration, and heading angles for precise control.

- **Obstacle Avoidance** also fall under two different categories
    - **Real-Time Detection:** Ensuring safety by detecting and avoiding obstacles in real-time.
    - **Reactive Navigation:** Uses sensors to make immediate adjustments, acting as a backup when the main autonomy system fails to detect obstacles.
