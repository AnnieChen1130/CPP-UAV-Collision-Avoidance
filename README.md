UAV-collision-avoidance
Collision avoidance algorithm developed by CPP UAV REU students

# CPP-UAV
File Structure 
1. CA.cpp is the main.cpp
2. autopilot_interface.cpp has all the funtions (autopilot, collision avoidance)
- Current ICAO of ADS-B for our aircraft: 3819648 
- Current ICAO of ADS-B for our quadcopter: 10700118

# To run the program in minicomputer
1. All hardwares have to turn on, please ask Aziz to help.
2. Open the terminal and go to the UAV project folder
3. If any new change has made to any file, use the command "make" first to compile the project
- if recevie error for "make" command:
*make: /snap/cmake/549/bin/cmake: Command not found
make: *** [Makefile:255: cmake_check_build_system] Error 127*
- Do "cmake + project path":
Example: *cmake ~/Documents/uav_project/UAV-collision-avoidance-master*
4. Command "sudo ./ CA" to run the program (sudo password: uavCPP2020)
5. to stop the running program, press Ctrl C in the keyboard.

# Mission Planner
First "Connect" at the right-up conner.

To set waypoints:
1. Go to "PLAN" at mission planner
2. click any area on the map to set the waypoints you want.
3. On the right hand side, there are options: "Read", "Write", "Write Fast". 
- Click "Write", then it will write to the program and send waypoints to mini computer

To see other aircraft's ADS-B (in case the setting is not saved)
1. Go to "CONFIG", and go to "Full Parameter List".
2. On the right hand side, search "adsb". Find "ADSB_Enable", change value to 1.
3. Search "Serial2", find "Serial2_Protocal", chang value to 2.
4. Search "select", find "ADSB_RF_Select", change value to 3.
5. After changed all the values, on the right hand side, click "Write Params" to save config. 

