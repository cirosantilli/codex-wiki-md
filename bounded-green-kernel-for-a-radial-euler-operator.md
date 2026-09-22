# Bounded Green kernel for a radial Euler operator

↑ **Parent:** [Green's function](green-s-function-split.md)

For $L y=(x^2y')'-2y$ on $x>0$, choose solutions bounded at zero and infinity. The homogeneous [Cauchy-Euler equation](cauchy-euler-equation.md) has basis $x,x^{-2}$. Joining the left-regular and right-regular solutions continuously and imposing $s^2[G_x]_{s^-}^{s^+}=1$ gives the displayed [Green's function](green-s-function-split.md) with ordinary integration measure $ds$. For bounded forcing,

$$
y(x)=-\frac1{3x^2}\int_0^x sf(s)ds-\frac x3\int_x^\infty\frac{f(s)}{s^2}ds.
$$

The integrals converge and give the unique bounded solution: no nonzero homogeneous combination is bounded at both ends. If $0\leq f\leq M$, negativity of the kernel gives $-M/2\leq y\leq0$. Differentiation cancels the two moving-endpoint terms, leaving

$$
y'(x)=\frac2{3x^3}\int_0^x sf(s)ds-\frac13\int_x^\infty\frac{f(s)}{s^2}ds,
$$

which implies $|y'(x)|\leq M/(3x)$. For constant forcing $f=M$, the bounded solution is $-M/2$; the endpoint conditions are boundedness, rather than zero endpoint values.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/8/solution.md)
