# Linear Regression  

## PROBLEM
    Predict the housing prices based on their area.
    
This problem is univariant linear regression problem, i.e. it only has one feature(x) and one lable(y) that corresponding to it. 
As we are building a linear regg. model so, we are trying to find a line or a function h(x) - Θ0 + Θ1*x for any x.

### Broad outline
    The data we have of with prices and area -- training data
                                                |-> Using it we create a model  
                                                    Housing area(x) ->  h(x)  -> Price of  the house.

#### So what we need to do is ---

- we must find the best values for c and m
    - such that the value (h(x(i)) - y(i)) is minimized 
- generally we define a cost function - J(Θ0,Θ1)) =1/(2n) * (1 -> m)Σ(h(x(i)) - y(i))² 
        we take the mean squared error here inorder to simplify

Cost Function 
- In order to find the minium value of c and m we must minimize the cost function
    - As for linear regression the we have taken squered  error the plot for J(Θ0,Θ1)) is a <u>elliptic paraboloid</u>
    - When we <u>differenciate</u> it we get a surface.
    - So if we move in the direction of negative desent we get the <u>minimum value of our J(Θ0,Θ1))</u> that is the vertex of the paraboloid.
