# Kinematics Simulation
Hi! Here's a user manual for this basic kinematics calculator and 2D projectile motion simulator I created for my grade 11 Physics ISP. This took quite a while to build and test, and while I have tested the system extensively, it may still be possible to trigger certain errors in very particular situations. Nevertheless, for students and teachers, this is a very valuable and engaging tool that simplifies and logically presents the potentially complicated concepts of kinematics and projectile situations and effectively applies the mathematics present in this unit.

### Calculator
In a kinematics situation with non-uniform motion and constant acceleration, there are five variables to consider when solving - acceleration, initial velocity, final (or current) velocity, displacement, and time. These five variables can describe an object's state at any point in time.

As the calculator page shows, there are five basic kinematics equations used to solve for these variables, and since each one excludes a certain one of these five variables, you only ever need three variables and some basic algebra to completely solve a kinematics problem.

When you use the calculator tool here, you first input any three of the five possible variables and then select which one you would like to solve for  and which to exclude - both of these should be distinct and not among the fields which you've inputted (i.e. you can't solve for acceleration if you've inputted it). From there, the program will parse your solve for and exclusion fields rearrange the corresponding equation from the set of five and use your inputted fields as parameters in the solving function to present you with an answer.

The program can account for many types of errors or invalid results. If you input the same variable for solve for and exclude or don't input values in enough fields, you'll be alerted. As well, if the program calculates a NaN result, it will display that there are no valid solutions: an example for this sort of situation is if you toss a ball that reaches a maximum displacement of 5m in the air and solve for when it will be 10m up - since that situation never occurs, the result is NaN. As well, all possible time results are shown (at an object's maximum displacement, the peak will be shown twice as it is the "double root" of the corresponding parabola), and if time results are invalid (below zero), that will be indicated when they are presented.

### Simulation
The simulation is a very complicated and fragile tool. It allows you to model 2D projectile motion where a projectile (shown always as a blue circle) has non-uniform vertical motion but uniform horizontal motion. In this simulation, positive movement values move up in the vertical plane and right in the horizontal plane and the canvas extends 280m in all cardinal directions from the canvas' center point (0 displacement).

To simulate a situation, you must input the correct amount of variables for both the x- and y-plane: only three of the following (y-acceleration, y-initial velocity, y-final velocity, y-displacement, and time) and two of the following (x-velocity, x-displacement, and time) should be inputted; time can count for both. Additionally, by changing the velocity input type tab to "Combined" instead of "Separate", you can represent y-initial velocity and x-velocity with a single vector with initial total velocity and direction in degrees above the horizontal - the program can use trigonometry to convert between these two forms. Keep in mind that you cannot represent only one of these two velocities with the "combined" option - this is relevant when accounting for inputting the correct number of variables.

Once the appropriate amount of variables have been inputted, click "Solve and Simulate!" and the ball on the canvas on the screen's left will follow the properties you've inputted - it will adjust to the displacement values and a "Step Interval" menu will appear below the canvas. From here, you can choose an interval of time (i.e. 0.5s) to step forward and backward in your simulation to see how the ball moves on the canvas and how its values change as the simulation progresses forwards or backwards.

This is an extremely powerful tool that is very useful in visualizing kinematics simulations and demonstrating the connections between the different variables (i.e. how the separate and combined velocity inputs connect). However, because the algorithm is quite complicated, it is possible to induce unfavourable behaviour under certain circumstances. Just as with the calculator, if invalid values are inputted, a NaN alert will appear that prevents the simulation from progressing. Additionally, the program is designed in such a way that time is always solved for last among the y-component variables, meaning that in situations where two time values are valid for a given displacement (such as an object moving upwards past 5m displacement and then coming back down crossing that 5m threshold again), only one time and final velocity situation will be presented - by experimenting with the simulation you can determine any additional situations that match those conditions.

### Conclusion
Thank you for checking out this tool - I hope it can be of great use to both students and teachers!