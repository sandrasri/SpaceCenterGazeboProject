# Gazebo Home Delivery Robot Simulation

## This is a simulation of a Gazebo Project that launches a smart home environment with two delivery robots operating inside the house.

### HOW TO LAUNCH
1. **Clone the repo:**   
   git clone
  
2. **Build the Plugin:**   
   mkdir build
   cd build
   cmake ..
   make

*This compiles the myworld.cpp file into a usable Gazebo plugin*   

3. **Export the Plugin Path**   
   export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/ubuntu/HouseGazeboProject/build

4. **Insert the Plugin into the World File**   
   cd world
   gedit dreamhouse.world

5. **Add the following line underneath the <world name="default"> tag in the file:**   
   <plugin name="myworld" filename="libmyworld.so"/>

6. **Run the simulation**   
   gazebo dreamhouse.world
   
