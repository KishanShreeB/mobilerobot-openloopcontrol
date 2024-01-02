# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1:

 Use from robomaster import robot

Step2:

Choose the x,y,z - axis movement distance(meters).

Step3:

 Give ep_chassis.move to move straight.

Step4:

 Give time.sleep() for a break.

Step5:

Give ep_chassis.drive_speed to have a circular movement.

## Program
```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.5, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=255,effect="on")

    ep_chassis.move(x=0.5, y=0, z=85, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")
    
    ep_chassis.move(x=0.70, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=0.35, y=0, z=90, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=255,effect="on")

    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=101,b=0,effect="on")
    
    ep_chassis.move(x=0, y=0, z=-40, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.63, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=143, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=51,b=102,effect="on")

    ep_chassis.move(x=0, y=1.55, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=51,b=102,effect="on")

    ep_chassis.move(x=2, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=128,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=82, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=0,b=225,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=225,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=225,effect="on")



    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
    
    ep_robot.close()

```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)


Insert image here
![WhatsApp Image 2024-01-02 at 23 46 28_f83d6e40](https://github.com/KishanShreeB/mobilerobot-openloopcontrol/assets/144870434/55a945c7-8cfc-4561-bfde-88555d27127a)
![WhatsApp Image 2024-01-02 at 23 46 27_543dcfac](https://github.com/KishanShreeB/mobilerobot-openloopcontrol/assets/144870434/ad267e51-e252-428e-a67b-52445b536016)
![WhatsApp Image 2024-01-02 at 23 46 28_ed858774](https://github.com/KishanShreeB/mobilerobot-openloopcontrol/assets/144870434/d708bc5b-f957-44f8-97f1-4cbeccb210d2)
![WhatsApp Image 2024-01-02 at 23 46 28_9c1bb0d4](https://github.com/KishanShreeB/mobilerobot-openloopcontrol/assets/144870434/25f5b54f-6f48-46e4-bb42-61b1630c3f06)


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)
https://youtu.be/dUtd1FnMlwY?si=_v3S-ukKMnpdri4x
<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
