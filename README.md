# Roundabout-Replication-Package
The pacakge includes the codes and simulation results related to the manuscript 'Evaluation of platooning configurations for connected and automated vehicles at an isolated roundabout in a mixed traffic environment'.
Main codes are written in python and matlab.
Here are the explanations for the 'Codes.rar'.
1. 'runner_flow.py' is the main code. Before running the code, you should download 'SUMO' simulation software, and create necessary files required by the 'SUMO', such as the 'road network' file, and the 'routes' file. The 'road network' file is created by using the embedded software in SUMO, by manually create a road networ. The 'routes' file is created by generating a xml file through the python code 'generateRoutes.py'. Besides, in 'runner_flow', you can change the three investigated platoon configurations, as described in the codes, including types of platoons, the maximum platoon size, and platoon willingness. The whole simulation step is also described in the manuscript.
2. 'generateRoutes.py' is for generating routes in your network. In this file, you can manually change the 'turning percentage', 'traffic flow', and 'penetration rate'.
3. 'output.py' is used for recording 'delay' and other metrics given by the 'SUMO'.
4. 'throughput.py' is used for recording 'throughput'.
5. 'storeInfo.py' is used for recording the number of platoons with different platoon sizes.
6. 'plot1.m' is used for creating the figures, such as Fig.5, Fig.6, etc. in the manuscript. This is written in 'Matlab'.
Here athe the explanations for the 'simulation results.rar'.
1. The results are recorded in the '.xlsx' format, and seperate them in terms of different penetration rates. For example, 'results_P=0.5.xlsx' stands for the results in the conditions of the penetration rate equalling 0.5. In the '.xlsx' file, it is further separated according to different 'turning percentages' and the investigated platoon configurations. For example, in the sheet 'platoon size(211)', it stands for the results generated in the conditions of the investigated platoon configuration is the maximum platoon size, and the turning percentage is [right,staright,left]=[0.5,0.25,0.25].
2. 'r2.xlsx' is for calculating the R-squared values, as described in the manuscript.
