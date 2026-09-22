# Bernstein linear programming hierarchy for polynomial minimization

↑ **Parent:** [Linear programming](linear-programming.md)

For $f$ of degree $d$ and $n\ge\max(1,d)$, compute its degree-$n$ [Bernstein basis](bernstein-basis.md) coefficients and solve $\max\lambda$ subject to $\lambda\le \beta_{k,n}$, $0\le k\le n$. This is a linear program with $n+1$ inequalities. The coefficients form a convex-combination enclosure of the polynomial values, so $v_n\le\min f$. [Degree elevation of Bernstein coefficients](degree-elevation-of-bernstein-coefficients.md) makes the bounds monotone. For every $\epsilon>0$, the polynomial $f-(\min f-\epsilon)$ is strictly positive, so [positive Bernstein coefficients for a strictly positive polynomial](positive-bernstein-coefficients-for-a-strictly-positive-polynomial.md) gives an eventual feasible bound $\min f-\epsilon$. Hence $v_n$ converges to the true minimum. Earlier indices $n<d$ can use a one-inequality program at any common coefficient-based lower bound, preserving the stated constraint count for every positive index.

## ↑ Ancestors (5)

1. [Linear programming](linear-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/3/d/solution.md)
