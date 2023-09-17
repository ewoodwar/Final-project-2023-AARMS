This project focuses on changes in population overtime with a spatially implicit model incorporating the Allee effect and Logistic model. 
    It is a two patch model depicting the rate of growth of invasive species in two lakes. The goal of the code provided gives is to give an insight into stability of the system and to answer our question. We first start by solving the two patch model which includes symmetric migration seen in equations (1) and (2). Due to the complexity of the system, it made sense to non-dimensionalize in order to reduce the number of parameters. In equation (1) and (2) we see there are 6 parameters, $(r,k,a_1,a_2,m_{12},m_{21})$, but after non-dimensionalization, we see the number of parameters is reduced down to 3, $(a_1,a_2,m)$. This makes finding the equilibria of the system easier. 
    
    We then evaluate the systems equilibrium points, which we find to be $(0,0)$. This was unexpected; we anticipated at least two equilibria. In order to find other equilibria, which may have not been captured the first time, we do a simple substitution to reduce the system of equations to one differential equation and find the equilibria from that. Doing it this way gives us a $9^{\text{th}}$ order polynomial for which we need to find the zeros, however the run time was extremely lengthy and we were not able to get the roots of the polynomial. 

    In order to find the stability of they system, we found the jacobian and plugged in the only equilibrium point we found, $(0,0)$. This point gives us an (DETERMINE TYPE OF SYSTEM) system. 

    Since we do not have actual parameters for the system, we constructed several phase planes by inputting different values for the 3 parameters. We can see the equilibrium points change as the parameters differ. The user is able to change the parameters at will in order to see the effects of the different values.

    Last we plot the nullclines associated with the phase planes. The parameters for the system proposed are quite difficult to find and hence, were unable to use the nullclines and phase planes to get further insight into answering our question, however, once again the user can change the values in order to see how the system changes. 
    
    In figures (INPUT FIGURE NUMBERS), we used the simple example of Spiney Flees along with initial conditions in order to plot the phase planes and nullclines. In order for the model to be exact, we must have correct parameters, but as mentioned above, we simply do not have the data to use in order to do further analysis of the system. 

    To answer our question of how we can use human induced Allee threshold in patch 1 to manage the spread of invasive species in patch 2, it is necessary to obtain parameter values of the species of interest, along with the correct initial conditions and be able to use numerical simulations. Further research would include conducting experiments or simulate data to get those parameters.
