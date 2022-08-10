# dandy_simulator
A simulation model to be used with the dandy robot software, specifically for hardware in the loop setups.

Install necessary gazebo and ros packages.

Ensure "use_sim_time" set to true for all nodes and node configurations.

Change Navsat Node: Remap imu topic from /imu/data/navsat to /imu/data and set wait for datum to false.

Comment out any sensor related nodes that gazebo will handle from launch file including diff drive nodes.

Run gazebo with: gazebo *world_file* -s libgazebo_ros_init.so 
