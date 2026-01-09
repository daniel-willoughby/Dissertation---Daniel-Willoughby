Installation
============

The release consists of three python programs

TrainingCamp.py          
TrainingCamp_lag.py
Inference.py

TrainingCamp.py is used to train policies
TrainingCamp_lag.py is a specialised version of TrainingCamp designed to implement policy lag
Inference.py is used to run inference on existing trained policy files

The libraries we used are documented in the requirements.txt file

Later versions of these libraries should run fine, the version numbers are 
provided as a reference showing the values used in the dissertation work.

Testing the Installation
========================

A simple first test would be to run two of our pre-trained policy files to observe them playing football

1.  Check the following files are in the default python project directory

policy_blue_lag_test.pt

policy_red_baseline_test.pt

2.  Run Inference.py.

3.  From the menu select ‘policy_blue_lag_test.pt’ as the blue policy.

4.  From the menu select 'policy_red_baseline_test.pt’ as the red policy.

5.  Select 5 games to be played

6.  You should at this point see the colour VMAS Football screen with 5 games being played.

7.  When the games finish a graph will be displayed showing the results

8.  The winning teams score will be displayed on the terminal output.

Training Policies
=================

1.  Edit the hyperparameters in TrainingCamp.py as required

2.  Run TrainingCamp.py 

3.  This training will take some time depending on parameters and will display training progress

4.  Two graphs will be displayed showing the how the teams have scored during the training 

5.  You will see two new  policy files in the project directory,  policy_blue.pt and policy_red.pt 

(NB Rename these files to something meaningful if you dont want them overwritten by the next training run)

6.  The policy files can then be used as inputs to Inference.py as shown above. 

