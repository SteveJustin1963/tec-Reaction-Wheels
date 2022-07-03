# tec-Reaction-Wheels

Reaction wheels are a type of flywheel used primarily by spacecraft for three-axis attitude control, which does not require rockets or external applicators of torque. They provide a high pointing accuracy, and are particularly useful when the spacecraft must be rotated by very small amounts, such as keeping a telescope pointed at a star. 


3 axis reaction wheel experiments

see also https://github.com/SteveJustin1963/tec-BALO



![image](https://user-images.githubusercontent.com/58069246/170595550-34e0d06a-9825-4c63-9120-dbe1b793ddda.png)
![image](https://user-images.githubusercontent.com/58069246/170595589-6a0c4cac-e6c4-41d4-8f46-9cd2d2f45820.png)
![image](https://user-images.githubusercontent.com/58069246/170595615-935431b6-9701-4f48-832a-c0a9deed46d9.png)
![image](https://user-images.githubusercontent.com/58069246/170595656-5fc0b312-a734-4ece-9c81-59aec13cf9d2.png)
![image](https://user-images.githubusercontent.com/58069246/170595833-137981ba-52f6-4f6c-990e-5d49c86dc1f4.png)
![image](https://user-images.githubusercontent.com/58069246/170595890-2e0fe9ed-43e9-4d12-8462-241dd8f7c12c.png)
![image](https://user-images.githubusercontent.com/58069246/170596254-fb66314b-e210-4c3b-9578-e83259d80c93.png)
![image](https://user-images.githubusercontent.com/58069246/170596357-586f44c4-5c8d-4dfb-bc32-bec1cae0e994.png)
![image](https://user-images.githubusercontent.com/58069246/170596848-299f7943-9fa7-47be-af87-20fffc65f30e.png)
![image](https://user-images.githubusercontent.com/58069246/170596517-d945ac69-c83b-4813-ae62-ad7fd4e97d31.png)
![image](https://user-images.githubusercontent.com/58069246/170598548-21942e81-8638-4ca6-938c-e6cab491e1ea.png)
![image](https://user-images.githubusercontent.com/58069246/170598200-e627d9fc-6a76-41f8-9385-dfc155d5ace7.png)

### Iterate
apply reaction wheels to tec-scope


There are a few ways to do this: 

1. Use a computer-controlled mount that has reaction wheels built in.

2. Use a separate set of reaction wheels mounted on the telescope itself.

3. Use a separate set of reaction wheels mounted on a platform that the telescope is sitting on.


## c code for 2 axis  reaction wheels, to point to a fixed location x,y
some basic code snippets that could be used in a two-axis reaction wheel system are provided below.

Assuming that the reaction wheels are already mounted, the first step would be to initialize them. This can be done by sending a signal to each wheel to start spinning in the desired direction. For example, to spin the wheels in the positive x and y directions, the following code could be used:

wheel1_spin(POSITIVE_X);

wheel2_spin(POSITIVE_Y);

Next, the wheels would need to be constantly monitored to make sure that they are pointing in the correct direction. This can be done by periodically checking the orientation of the spacecraft and comparing it to the desired orientation. If its not pointing in the correct direction, the wheels would need to be adjusted accordingly. For example, if its pointing in the negative x direction, the following code could be used to adjust the wheels:

wheel1_spin(NEGATIVE_X);

wheel2_stop();

Finally, once its pointing in the correct direction, the reaction wheels can be turned off. This can be done by sending a signal to each wheel to stop spinning. For example, the following code could be used to stop the wheels:

wheel1_stop();

wheel2_stop();
; end




### Ref
- https://en.wikipedia.org/wiki/Reaction_wheel
- https://www.rocketlabusa.com/satellite-components/reaction-wheels/
- https://charleslabs.fr/en/project-Reaction+Wheel+Attitude+Control
- https://hackaday.com/2022/04/27/building-reaction-wheels-with-python-and-lego/
- https://www.youtube.com/watch?v=woCdjbsjbPg
- https://github.com/CGrassin/reaction_wheel

