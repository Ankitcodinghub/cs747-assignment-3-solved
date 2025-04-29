# cs747-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [CS747 Assignment 3 Solved](https://www.ankitcodinghub.com/product/cs-747-programming-assignment-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;109974&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS747 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
This assignment tests your understanding of the concepts taught in class and its applications to real world problems. In particular, we examine one of the most popular domains: autonomous driving. You will have to come up with a controller to drive a car, and are free to use any approach: coding it up yourself and/or learning with value function-based approaches and/or using policy search.

There are two tasks in this assignment. In Task 1, you will construct a controller that can navgiate a car out of a parking lot on a winter night. The surroundings are icy and the parking lot is also close to freezing. It is your responsibility to get the car out of this situation and on the road safely. Task 2 is along similar lines but you find yourself in a stickier situation. The parking lot is now filled with pools of mud from a cold winter storm. You must dodge these obstacles and find a safe way out.

All the code you write for this assignment must be in Python 3.8.10. The libraries that you require come installed with the docker image that has been shared for the course, and are already imported in the files you need to complete.

Code Structure

This compressed directory has all the files and folders that are required for the assignment (we acknowledge Wesley Hsieh for a base simulator that our assignment is built upon). For the most part, you do not need to worry about these files. It is, however, advised that you read through driving_env.py in the envs folder to understand how the _step function works. In short, it returns the reward, termination condition, the next state and a boolean flag to indicate the success of the episode (it also returns a dictionary with additional information that can be ignored). In addition to the above, the _reset function of the simulator resets the environment and returns the initial state of the car.

We have provided run_simulator.py to run simulations and visually see the working of your controller, which you’ll have to submit as described later. This code has been provided with 10 random seeds that evaluate your controllers for a fixed few environments (different initial states of your car and different positions of the obstacles in Task 2) and outputs the execution time. The only file you need to edit is run_simulator.py. Do not edit any other files.

For evaluation, we will use another set of environments in the autograder, and use its score as is for the evaluation. See the exact details below.

Task 1: The Parking Lot Problem

As mentioned above, your task is to navigate your 50 x 25 car out of a 700 x 700 square grid. It must exit onto the road whose entrance has its centre located at (350, 0). This grid is centred at the origin with the coordinate axes shown below (screen size: 1000 x 1000). It is an episodic task that begins with your car initialised at a random position and orientation; the episode ends when you navigate out or bump into a wall (or pit in Task 2). We also cap episodes to a total of 1000 time steps.

Your car has 4 state features: the x and y position coordinates, the velocity and the heading angle. In order to control the state, you have two independent control inputs steer and acceleration that take the following discrete values.

Control Input: Steer

0 -3 degrees

1 0 degrees

2 3 degrees

Task 2: The Parking Lot Problem Intensifies

Building on the first task, your goal now is still to navigate your 50 x 25 car out of a 700 x 700 square grid. It must exit onto the road whose entrance has its centre located at (350, 0). However, this time, the road is narrower and the parking lot is filled with 4 randomly located pits of mud (with a size of 100 x 100 each). The parking lot is once again centred at the origin with the coordinate axes shown below (screen size: 1000 x 1000).

Running the Code

Since it is important for you to be able to visualise your agent’s behaviour as you develop it, we had provided a visual interface. However, this might not run as is on the docker, and you will have to run the code on your local system so that a new game window is allowed to open with the render_mode flag. Without the flag, however, since there will be no rendering, you can run your code in the docker container. If you want to run on your local system, you just have to run pip install -e

. from the root directory gym_driving_dir so that the dependencies from setup.py get installed automatically before you run the scripts. To run on docker, however, you will need to follow additional steps. Firstly, run pip install -e . from the root directory gym_driving_dir as before (do not worry if some warnings are given). From within the docker, running OpenCV throws an error ImportError: libGL.so.1: cannot open shared object file: No such file or directory. To circumvent this, you have to install libgl1 by apt-get update &amp;&amp; apt-get install libgl1 .

To run the code you have written run python run_simulator.py –task T1/T2 –render_mode (use this while running code in your local system as mentioned) to visualise the simulation and python run_simulator.py –task T1/T2 (only this command will work inside docker) otherwise from the simulator directory.

Now to verify the code against the 10 random seeds run python autograder.py –task T1/T2 from the simulator directory. To pass the autograder, you should not put any additional print statements in the code (comment them out if you used them for debugging). Evaluation

Submission
