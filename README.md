#Usage
Here is a quick sum up of the last step from the tutorial http://gazebosim.org/tutorials?tut=plugins_model. 

Prepare for build and build the module
```bash
mkdir build
cd build
cmake ..
make
cd ..
```

Do not forget to execute this line each time you open a new terminal (with your own path).
```bash
export GAZEBO_PLUGIN_PATH=$HOME/catkin_ws/src/control_pipeline/gazebo_plugin_tutorial/build:$GAZEBO_PLUGIN_PATH
```

To make this plugging working alone, you can start it with the command
```bash
gzserver -u model_push.world
```

And start gazebo with
```bash
# for gazebo only:
gzclient

# OR for Ascend setup in gazebo:
$ roslaunch main.launch
```

Then we should be able to interact with the drone by calling
```bash
$ rosrun fluid example_client.py
```

But it crasheeeees...
takk hvis noen kan hjelpe!
