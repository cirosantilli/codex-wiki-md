<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $s=Z+c\theta$ and write $q=Q(s)$. Substitution into the [modified Burgers equation with cubic flux](../../../../../../modified-burgers-equation-with-cubic-flux.md) gives

$$
(1-cQ^2)Q'=\epsilon c^2Q''.
$$

After one integration,

$$
\epsilon c^2Q'=Q-\frac c3Q^3+C.
$$

A regular constant limiting state has $Q'\to0$. The state $Q=0$ at the negative end sets $C=0$, and the nonzero state $Q=\beta$ at the positive end gives

$$
\boxed{c=\frac3{\beta^2}.}
$$

Thus the first-order equation is $\epsilon c^2Q'=Q(1-Q^2/\beta^2)$. Put $W=Q^2$. Its equation is logistic,

$$
W'=\frac2{\epsilon c^2}W(1-W/\beta^2).
$$

The heteroclinic [travelling wave](../../../../../../travelling-wave.md) connecting the prescribed endpoints is consequently

$$
\boxed{q(\theta,Z)=\frac{\beta}{\sqrt{1+\exp[-2(Z+c\theta-s_0)/(\epsilon c^2)]}},\qquad c=3/\beta^2,}
$$

where $s_0$ is an arbitrary translation. Taking the sign from $\beta$ is essential; squaring the equation alone loses the negative-front solution. A fixed level propagates with $d\theta/dZ=-1/c=-\beta^2/3$, also obtained from the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md) for flux $-q^3/3$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
