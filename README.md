# carla_urop
Carla UROP files for birdeye view

move_forward.py is file that sets throttle to a certain speed and sets the direction to forward.
I created this file after setting up the simulator and scenario runner folder.
I did this by editing the manual_control.py file that was in the scenario_runner folder.
To set the throttle I use the .control.throttle = .8 command. This set the vehicle to 80% of the max throttle.
Once I saw that the car constantly moved forward I tried to get the birdeye-view working. Following the directions
in the documentation I used pip install carla-birdeye-view to install tha package. Then, I used the code provided in the
basic code usage setion to seee the output arrays. I imported the libraries at the top of the move_forward file. I put the 
three lines of code provided on the birdeye page inside of the while loop in the game loop function of the move_forward file. 
When running, I would first launch carla using the./CarlaUE4.sh command and then I would launch the move_forward file. Finally, 
I would run the sudo python3 -m carla_birdeye_view command from the bireye command. I had to add the sudo and use python3 
instead of just python so the command would execute. This would eventually cause a small window to open that was labelled BirdView RGB,
but the window was just a white rectangle.
