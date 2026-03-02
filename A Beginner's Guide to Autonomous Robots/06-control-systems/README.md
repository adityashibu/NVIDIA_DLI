# Control Systems in Robotics

Once a robot's trajectory and target states are defined, the control system translates this information into commands for the robot's actuators. This ensures that the robot follows the planned path accurately.

## Feedback Control

**Feedback control** adjust the robot's actions based on sensor feedback to achieve desired behaviors. A common method for feedback control is **PID (Proportional-Integral-Derivative) control**. 

PID is a widely used algorithm that minimizes the error between desired and actual positions by continuously adjusting movements. It operates by comparing the desired trajectory states with actual states obtained from localization data and making real-time corrections.

## Trajectory Tracking

**Trajectory Tracking** is used to ensure that the robot accurately follows the planning path. One common algorithm used for this is MPC **(Model Predictive Control)**. 

MPC is an advanced control algorithm that optimizes the robot's path using a predictive model of its behavior. MPC is more complex than PID control and is often used for precise trajectory tracking and whole-body control in humanoid robots.
