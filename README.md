UAV-collision-avoidance
Collision aovidance algorithm developed by CPP UAV REU students

Current ICAO of ADS-B in Piper Cub aircraft: 3819648
Current ICAO of ADS-B on test board: 10700118

# CPP-UAV
File Structure 
1. CA.cpp is the main.cpp
2. autopilot_interface.cpp has all the funtions (autopilot, collision avoidance)

To run the program in minicomputer
1. All hardwares have to turn on, please ask Aziz to help.
2. Open the terminal and go to the UAV project folder
3. If any new change has made to any file, use the command "make" first to compile the project
- if recevie error for "make" command:
*make: /snap/cmake/549/bin/cmake: Command not found
make: *** [Makefile:255: cmake_check_build_system] Error 127*
-Do "cmake + project path":
Example: *cmake ~/Documents/uav_project/UAV-collision-avoidance-master*
4. Command "sudo ./ CA" to run the program (sudo password: uavCPP2020)
5. to stop the running program, press Ctrl C in the keyboard.
