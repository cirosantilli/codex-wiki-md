<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute the [power series](../../../../../../power-series.md) into $(1-x^2)y''-2xy'+\lambda y=0$. The coefficient of $x^k$ is $(k+2)(k+1)a_{k+2}+[\lambda-k(k+1)]a_k$, so

$$
\boxed{a_{k+2}=-\frac{\lambda-k(k+1)}{(k+1)(k+2)}a_k.}
$$

Starting from $a_0,a_1$ determines the even and odd coefficient sequences separately. Unless a sequence terminates, the ratio of successive same-parity coefficients has absolute value tending to one, so its series converges for $|x|<1$ and solves the [Legendre differential equation](../../../../../../legendre-differential-equation.md) there.

With $\lambda=n(n+1)$, choose the parity matching $n$ and set the other starting coefficient to zero. All factors before index $n$ are nonzero, whereas the factor at $k=n$ vanishes. Thus the chosen series is a nonzero polynomial of exactly degree $n$. Its value at one cannot vanish: a zero of multiplicity $j\ge1$ there would give a nonzero leading term $-2j^2(x-1)^{j-1}$, times its local leading coefficient, in the differential equation. We can therefore scale it to $P_n(1)=1$.

For $n=2$, $a_1=0$, $a_2=-3a_0$, and all later coefficients vanish. Normalization gives $a_0=-1/2$, yielding

$$
\boxed{P_2(x)=\frac12(3x^2-1).}
$$

For even degree this scale is fixed by $a_0$ as in the question; for odd degree $a_0=0$ by parity and the scale is fixed by $a_1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
