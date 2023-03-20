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

### The first root (2)

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

### The second root (${\approx -3}$)

From the graph, we can tell that there is also a root somewhere around -3.

The Newton-Raphson method performs extraordinarily better than the Bisection method when the former is given values that are far from the intended root and the latter given intervals that are spread far apartm regardless of whether the intended root is within the interval or not.

An example is when, for the same polynomial above, the Newton-Raphson method is done using an initial guess of -10000 and the bisection method is done using the interval ${(-200, 100)}$

> **Bisection**

    Time: 50594.50629999992ms

    Iterations: 10000000 (And still the root is not found!)

> **Newton-Raphson**

    Time: 0.9284999978262931ms

    Iterations: 33 (Root approximated as x = -3.156185)
