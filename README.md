# dandy_simulator
A simulation model to be used with the dandy robot software, specifically for hardware in the loop setups.

Install necessary gazebo and ros packages.
Ensure to set "use_sim_time" to true for all nodes.
Change Navsat Node imu remap from /imu/data/navsat to imu/data
Comment out any sensor related nodes that gazebo will handle from launch file
Run gazebo with: gazebo *world_file* -s libgazebo_ros_init.so 
