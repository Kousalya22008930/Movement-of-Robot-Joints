# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)

```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/Kousalya22008930/Movement-of-Robot-Joints/assets/119389108/5071bd6e-9205-42bf-aab4-f012c91bfb08)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Kousalya22008930/Movement-of-Robot-Joints/assets/119389108/99510fe6-6ece-46eb-a491-5a89ab4fbdf5)

### 3. Movement of Joint1
![image](https://github.com/Kousalya22008930/Movement-of-Robot-Joints/assets/119389108/6762553a-8648-4d2e-b1d3-611f1a57dfa1)

### 4. Movement of Joint2
![image](https://github.com/Kousalya22008930/Movement-of-Robot-Joints/assets/119389108/125252a8-abfa-45ca-85ae-e027dc4ed525)

### 5. Movement of Joint3
![image](https://github.com/Kousalya22008930/Movement-of-Robot-Joints/assets/119389108/40b87eed-ec4d-4eef-bf62-ea712de9f6f5)



## Result 
Thus the different robots joints are moved with the help of python list.


