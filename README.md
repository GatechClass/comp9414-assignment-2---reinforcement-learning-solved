# comp9414-assignment-2---reinforcement-learning-solved
**TO GET THIS SOLUTION VISIT:** [COMP9414 Assignment 2 – Reinforcement Learning Solved](https://mantutor.com/product/comp9414-24t2-solved-2/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114859&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP9414 Assignment 2 - Reinforcement Learning Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Artificial Intelligence

Assignment 2 – Reinforcement Learning

1 Problem context

Taxi Navigation with Reinforcement Learning: In this assignment, you are asked to implement Q-learning and SARSA methods for a taxi navigation problem. To run your experiments and test your code, you should make use of the Gym library , an open-source Python library for developing and comparing reinforcement learning algorithms. You can install Gym on your computer simply by using the following command in your command prompt:

pip install gym

In the taxi navigation problem, there are four designated locations in the grid world indicated by R(ed), G(reen), Y(ellow), and B(lue). When the episode starts, one taxi starts off at a random square and the passenger is at a random location (one of the four specified locations). The taxi drives to the passenger’s location, picks up the passenger, drives to the passenger’s destination (another one of the four specified locations), and then drops off the passenger. Once the passenger is dropped off, the episode ends. To show the taxi grid world environment, you can use the following code:

env = gym.make(”Taxi−v3” , render mode=”ansi ”). env

state = env . reset () rendered env = env . render () print ( rendered env )

In order to render the environment, there are three modes known as “human”, “rgb array, and “ansi”. The “human” mode visualizes the environment in a way suitable for human viewing, and the output is a graphical window that displays the current state of the environment (see Fig. 1). The “rgb array” mode provides the environment’s state as an RGB image, and the output is a numpy array representing the RGB image of the environment. The “ansi” mode provides a text-based representation of the environment’s state, and the output is a string that represents the current state of the environment using ASCII characters (see Fig. 2).

Figure 1: “human” mode presentation for the taxi navigation problem in Gym library.

You are free to choose the presentation mode between “human” and “ansi”, but for simplicity, we recommend “ansi” mode. Based on the given description, there are six discrete deterministic actions that are presented in Table 1.

For this assignment, you need to implement the Q-learning and SARSA algorithms for the taxi navigation environment. The main objective for this assignment is for the agent (taxi) to learn how to navigate the gird-world and drive the passenger with the minimum possible steps. To accomplish the learning task, you should empirically determine hyperparameters, e.g., the learning rate α, exploration parameters (such as ϵ or T), and discount factor γ for your algorithm. Your agent should be penalized -1 per step it

Figure 2: “ansi” mode presentation for the taxi navigation problem in Gym library. Gold represents the taxi location, blue is the pickup location, and purple is the drop-off location.

Table 1: Six possible actions in the taxi navigation environment.

Action Number of the action

Move South 0

Move North 1

Move East 2

Move West 3

Pickup Passenger 4

Drop off Passenger 5

takes, receive a +20 reward for delivering the passenger, and incur a -10 penalty for executing “pickup” and “drop-off” actions illegally. You should try different exploration parameters to find the best value for exploration and exploitation balance.

After training your algorithm, you should save your Q-values. Based on your saved Q-table, your algorithms will be tested on at least 100 random grid-world scenarios with the same characteristics as the taxi environment for both the Q-learning and SARSA algorithms using the greedy action selection

Figure 3: Q-learning reward. Figure 4: Q-learning steps.

Figure 5: SARSA reward. Figure 6: SARSA steps.

method. Therefore, your Q-table will not be updated during testing for the new steps.

Your code should be able to visualize the trained agent for both the Qlearning and SARSA algorithms. This means you should render the “Taxiv3” environment (you can use the “ansi” mode) and run your trained agent from a random position. You should present the steps your agent is taking and how the reward changes from one state to another. An example of the visualized agent is shown in Fig. 7, where only the first six steps of the taxi are displayed.

2 Testing and discussing your code

Before your discussion session, you should prepare the necessary code for this purpose by loading your Q-table and the “Taxi-v3” environment. You should be able to calculate the average number of steps per episode and the

Figure 7: The first six steps of a trained agent (taxi) based on Q-learning algorithm.

average accumulated reward (for a maximum of 100 steps for each episode) for the test episodes (using the greedy action selection method).

3. Fair, 2. Low, 1. Deficient, 0. No answer.

Results obtained from agent learning

Results obtained from testing the trained agent

Code understanding and discussion

Code readability for Q-learning algorithm 1 mark

Code readability for SARSA algorithm 1 mark

Code understanding and discussion for Q-learning algorithm 5 mark

Code understanding and discussion for SARSA algorithm 5 mark

3 Submitting your assignment

Although we try to answer questions as quickly as possible, we might take up to 1 or 2 business days to reply, therefore, last-moment questions might not be answered timely.

3.

Table 3: COMP9414 24T2 Tutorials

1 4210 Fri 12:00 – 14:00 Siti Mariyah s.mariyah@unsw.edu.au

2 4211 Fri 12:00 – 14:00 Malhar Patel malhar.patel@unsw.edu.au

3 4212 Fri 14:00 – 16:00 Stefano Mezza s.mezza@unsw.edu.au

4 4213 Fri 14:00 – 16:00 Janhavi Jain j.jain@student.unsw.edu.au

5 4214 Fri 14:00 – 16:00 Adam Stucci a.stucci@unsw.edu.au

6 4215 Fri 16:00 – 18:00 Janhavi Jain j.jain@student.unsw.edu.au

7 4216 Fri 18:00 – 20:00 Jingying Gao jingying.gao@unsw.edu.au

8 4217 Thu 14:00 – 16:00 Shengyuan Xie shengyuan.xie@student.unsw.edu.au

9 4218 Thu 14:00 – 16:00 Adam Stucci a.stucci@unsw.edu.au

10 4219 Thu 14:00 – 16:00 Malhar Patel malhar.patel@unsw.edu.au

11 4220 Thu 16:00 – 18:00 Siti Mariyah s.mariyah@unsw.edu.au

12 4221 Thu 18:00 – 20:00 Jingying Gao jingying.gao@unsw.edu.au

13 4223 Tue 09:00 – 11:00 Zahra Donyavi z.donyavi@unsw.edu.au

14 4224 Tue 12:00 – 14:00 Maher Mesto m.mesto@unsw.edu.au

15 4225 Tue 12:00 – 14:00 Raktim Kumar Mondol r.mondol@unsw.edu.au

16 4226 Tue 12:00 – 14:00 Stefano Mezza s.mezza@unsw.edu.au

17 4227 Tue 16:00 – 18:00 Shengyuan Xie shengyuan.xie@student.unsw.edu.au

18 4228 Tue 16:00 – 18:00 Zahra Donyavi z.donyavi@unsw.edu.au

19 4229 Tue 16:00 – 18:00 Raktim Kumar Mondol r.mondol@unsw.edu.au

20 4230 Tue 16:00 – 18:00 Aayush Gupta aayush.gupta@unsw.edu.au

21 4231 Tue 18:00 – 20:00 Aayush Gupta aayush.gupta@unsw.edu.au

22 4232 Wed 09:00 – 11:00 Kiran Jeet Kaur kiran jeet.kaur@student.unsw.edu.au

23 4233 Wed 13:00 – 15:00 Stefano Mezza s.mezza@unsw.edu.au

24 4234 Wed 13:00 – 15:00 Kiran Jeet Kaur kiran jeet.kaur@student.unsw.edu.au

25 12564 Wed 12:00 – 14:00 Lina Phaijit l.phaijit@unsw.edu.au

26 12565 Tue 16:00 – 18:00 Zhijin Meng zhijin.meng@student.unsw.edu.au

27 12696 Thu 18:00 – 20:00 Ramya Kumar ramya.kumar1@student.unsw.edu.au

28 12695 Tue 18:00 – 20:00 Maher Mesto m.mesto@unsw.edu.au

29 12693 Wed 18:00 – 20:00 Zhijin Meng zhijin.meng@student.unsw.edu.au

30 12694 Wed 18:00 – 20:00 Ramya Kumar ramya.kumar1@student.unsw.edu.au
