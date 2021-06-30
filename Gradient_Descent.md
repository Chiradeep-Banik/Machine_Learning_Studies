# Gradient Descent 

Function in the linear regression problem 

    h(x(i)) = Θ0 + Θ1*x(i)

Cost Function 

    J(Θ0,Θ1)) =1/(2n) * (1 -> m)Σ(h(x(i)) - y(i))²

All this boil down to our gradient descent algorithm, that allows us to minimize our cost function and give us the best values for Θ0 and Θ1

    repeat till converges {
        Θj := Θ0 - α*partial_differenciation(J(Θ0,Θ1))       [ α -> Learning Rate, j = 0 and j = 1]
    }
    Learning Rate : Is the step size by which the cost function changes its value

#### In the Gradient Descent algorithm 
- We start at a point where we calculate the cost function.
- Then we start finding the direction to go, so that the cost function decreases.
- This allows us to move towords the local optimum where the cost function is at its minimum
- There the gradient discent stops as it has converged, i.e. Θj is the same as we calculate from the function 

This is also known as Batch Gradient Descent Algorithm -- as it calcultes the whole batch, i.e. Σ(1->m)

For learning rate 
- α can be fixed -- the function will <u>converge</u>
- α can be a small value -- the function would take more time but will <u>converge</u>
- α can be a large value -- the function may converge od <u>diverge</u>
- α can be changing -- it can decrease as we come closer to the local optimum. It will be <u>faster</u>

