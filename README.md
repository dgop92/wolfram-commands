# Wolfram Commands CheatSheet

## Basic Algebra

Partial Fractions
```
Apart[(x^2-4)/(x^4-x)]
```

Simplify
```
Simplify[1/6 n (19 + 15 n + 2 n^2)]
```

## Basic Calculus

### Derivatives

```
D[2x]
D[2x, x]
D[2xy, y]
D[2x^2y, x, y]
```

### Indefinite Integrals

```
Integrate[2x]
Integrate[2x, x]
Integrate[2xy, y]
Integrate[2x^2y, x, y]
```

### Definite Integrals
```
Integrate[2x,{x,0,5}]
Integrate[2yx,{y,0,5}]
Integrate[Integrate[2yx,{y,0,5}], {x, 5, 4}]
```

## Linear Algebra

### Dot Product

```
Dot[{1, 2}, {3, 4}]
Dot[{t, t^2}, {2t, 1}]
```

### Determinant

```
Det[{1, 2}, {3, 4}]
Det[{t, t^2}, {2t, 1}]
```

### Norm

```
Norm[{1,2}]
Norm[{t^3,5t}]
```

## Extras
```
Curl[-y/(x^2+y^2), -x/(x^2+y^2), z]
```

### Differential Equation

Check if a function is a solution of the equation, if the result is 0 that means is a solution
```
Simplify (D[#, x] + 3# - e^(2x))& @ (e^(2x)/5)

e^(2x)/5 = function to test
D[#, x] + 3# - e^(2x) = differential equation

```

Find potential function
```
Dsolve[{D[u[x, y], x],D[u[x, y], y]} == {f(x,y),g(x,y)}, u[x,y], {x,y}]
vectorial field = F(f(x,y), g(x,y))
```