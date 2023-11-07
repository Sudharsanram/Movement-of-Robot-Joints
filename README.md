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
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot

![280909006-bb9370e6-7ecf-4a5d-8805-7ddb9de9f1f7](https://github.com/Sudharsanram/Movement-of-Robot-Joints/assets/119393980/bfebaea4-2830-48b4-9781-075ad33076ba)

### 2. robot.driveJoints(0,0,0,0,0,0)

![280909050-449dea70-d689-4847-b69b-73903e2321a3](https://github.com/Sudharsanram/Movement-of-Robot-Joints/assets/119393980/84d2523c-18f6-4ef1-8d05-d47c1170f3c3)


### 3. Movement of Joint1

![280909084-9dd310e1-88ed-4936-a484-45a458472079](https://github.com/Sudharsanram/Movement-of-Robot-Joints/assets/119393980/98b02d20-1c00-4ad1-ba23-7e22cac35fca)

### 3. Movement of Joint2

![280909138-a78b703e-f79e-413d-ad1f-c8d3a3965076](https://github.com/Sudharsanram/Movement-of-Robot-Joints/assets/119393980/c9b9fcea-c231-48dc-8057-4285a3468c8e)



### 3. Movement of Joint3

![280909163-1da6b34f-6081-4a09-ac00-69f3c15affad](https://github.com/Sudharsanram/Movement-of-Robot-Joints/assets/119393980/3edb2951-2d99-4db6-a6b1-6ea8e04bd73b)

## Result 
Thus the different robots joints are moved with the help of python list.


