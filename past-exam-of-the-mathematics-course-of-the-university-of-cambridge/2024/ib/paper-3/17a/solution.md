<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

If the bound is to hold with finite $c$, the error functional must vanish on every [polynomial](../../../../../polynomial-split.md) whose fourth [derivative](../../../../../derivative.md) is zero. Thus the scheme must be exact for degrees zero through three. Applying it to powers of $t=x+1$ gives

$$
\begin{aligned}
a_{-1}+a_0+a_1+a_2&=0,\\
a_0+2a_1+3a_2&=0,\\
a_0+4a_1+9a_2&=2,\\
a_0+8a_1+27a_2&=0.
\end{aligned}
$$

Solving,

$$
\boxed{a_{-1}=2,
\qquad a_0=-5,
\qquad a_1=4,
\qquad a_2=-1}.
$$

This is the [four-point one-sided second-derivative formula](../../../../../four-point-one-sided-second-derivative-formula.md).

The [Peano kernel theorem](../../../../../peano-kernel-theorem.md) says that if a linear functional $L$ annihilates all [polynomials](../../../../../polynomial-split.md) of degree below $r$, then for $f\in C^r[a,b]$,

$$
L(f)=\int_a^bK(t)f^{(r)}(t)\,dt,
\qquad
K(t)=L\left(\frac{(x-t)_+^{r-1}}{(r-1)!}\right).
$$

Here $r=4$ and $L=e$. Under the stated nonnegativity assumption,

$$
|e(f)|\leq
\left(\int_{-1}^2K(t)\,dt\right)
\max_{[-1,2]}|f^{(4)}|.
$$

The [integral](../../../../../integral.md) equals $e(q)$ for $q(x)=(x+1)^4/24$, since $q^{(4)}=1$. Now $q''(-1)=0$ and

$$
\eta(q)=\frac{-5+4\cdot16-81}{24}=-\frac{11}{12}.
$$

Therefore

$$
\int_{-1}^2K(t)\,dt=e(q)=\frac{11}{12}.
$$

Equality is attained by $q$, so the [sharp Peano-kernel constant for the four-point endpoint second derivative](../../../../../sharp-peano-kernel-constant-for-the-four-point-endpoint-second-derivative.md) is

$$
\boxed{c=\frac{11}{12}}.
$$

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
