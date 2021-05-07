# ROS-Speech-Recognition-and-Speech-Synthesis
A robot self introduction example when prompted by user via speech

This is one of the assignments in the RoboCup@Home Education ROS Open Robot Platform learning class, where users speak into the microphone for the script to recognize the words and respond initially with the said words, 
modified into a script where the robot can respond with a self-introduction when prompted with keywords(using keyword spotting mode).

Methods to use(Assuming ROS is installed and setup correctly):
1. Run 'roscore' in a node
2. Run 'roslaunch rchomeedu_speech lm.launch' 
   - The arguments are specified in the launch file and can be modified to include from the command line
3. Run 'rostopic echo /robocup_qna' 
   - The name of the topic can be changed in the lm-test.py file
   - This is to read from the topic that the previous node has published to
4. Run 'roslaunch rchomeedu_speech talkback.launch' 
   - This is the file where the response can be modified to speak the said words, or custom made to respond uniquely
   
   
