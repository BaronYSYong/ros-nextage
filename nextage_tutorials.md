# Nextage Tutorial

## Webpage
* http://wiki.ros.org/rtmros_nextage/Tutorials
* http://wiki.ros.org/rtmros_nextage/Tutorials/Programming_Hiro_NEXTAGE_OPEN_RTM

## Install NEXTAGE Open 
http://wiki.ros.org/rtmros_nextage/Tutorials/Install%20NEXTAGE%20OPEN%20software%20on%20your%20machine

```
$ sudo apt-get update && sudo apt-get install ros-indigo-rtmros-nextage ros-indigo-rtmros-hironx
$ rtmlaunch nextage_ros_bridge nextage_ros_bridge_simulation.launch
$ rtmlaunch hironx_ros_bridge hironx_ros_bridge_simulation.launch   (HIRO)
$ rtmlaunch nextage_ros_bridge nextage_ros_bridge_simulation.launch (NEXTAGE OPEN)
```

## Command
* setTargetPose('rarm', [0.32, -0.18, 0.06], [-3, -1.5, 3.0], tm=3)
* setTargetPoseRelative('rarm', 'RARM_JOINT5', dz=0.01, tm=3)
* getCurrentPosition('RARM_JOINT5')
* getCurrentRPY('RARM_JOINT5')
* setJointAngle(self, jname, angle, tm)
* setJointAngles(self, angles, tm)
* setJointAnglesOfGroup(self, gname, pose, tm, wait=True)
* getJointAngles(self)

## Reference
* /opt/ros/indigo/lib/python2.7/dist-packages/hironx_ros_bridge
* /opt/ros/indigo/lib/python2.7/dist-packages/nextage_ros_bridge
* /opt/ros/indigo/lib/python2.7/dist-packages/hrpsys/hrpsys_config.py
* /opt/ros/indigo/share/nextage_ros_bridge/script/nextage.py
