<h1 id="1a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The forcing base $-2$ is a root of the [characteristic equation of a linear recurrence](../../../../../../characteristic-equation-of-a-linear-recurrence.md), so a constant multiple of $(-2)^n$ cannot be a [particular solution](../../../../../../particular-solution.md). For $P(r)=r^3-3r+2$, direct substitution gives

$$
L[nr^n]=r^n\bigl(nP(r)+rP'(r)\bigr).
$$

For the resonant case of [exponential forcing in a linear recurrence](../../../../../../exponential-forcing-in-a-linear-recurrence.md), at $r=-2$, $P(-2)=0$ and $(-2)P'(-2)=-18$. Hence $-(n/18)(-2)^n$ is a [particular solution](../../../../../../particular-solution.md) of the [inhomogeneous linear recurrence](../../../../../../inhomogeneous-linear-recurrence.md). **The general solution is**

$$
\boxed{y_n=A+Bn+C(-2)^n-\frac n{18}(-2)^n.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1A](../../1a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
