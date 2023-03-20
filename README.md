# Numerical Analysis Assignment

Name: Omondi Glen Ochieng
Reg-no: SCT211-0035/2021

## Newton-Raphson method vs Bisection method

The equation used for in both of the methods is:

${f(x) = x^4+ 2x^3 + x^2 + 2x - 40}$

Its derivative is:

${\dfrac{df}{dx} = 3x^3 + 6x^2 + 2x + 2}$

The graph of the equation is as shown
![graph](graph.jpg)

As it is possible to see from the graph, one of the roots of the equation is exactly 2. Both of the methods realized this value, given the parameters that were passed into it.

The Bisection method, in this case performed better than the Newton-Raphason method with the statistics shown below for 1 execution of each:

> **Bisection**

    Time: 0.1978999998755171ms

    Iterations: 26

> **Newton-Raphson**

    Time: 0.6138999997347128ms

    Iterations: 6

This was so because of the well-chosen interval ${ (1, 4) }$ which is relatively close to 2, one of the desired roots.

It is also interesting to note that although the bisection method took more iterations to arrive at the root, it still completed faster than the Newton-Raphson method in this case.
