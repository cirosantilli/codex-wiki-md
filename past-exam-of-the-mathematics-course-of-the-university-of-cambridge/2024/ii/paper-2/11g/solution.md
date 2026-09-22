<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

Put $A_j=\left(\begin{smallmatrix}a_j&b_j\\1&0\end{smallmatrix}\right)$. The identity

$$
A_0\cdots A_n=
\begin{pmatrix}p_n&b_np_{n-1}\\q_n&b_nq_{n-1}\end{pmatrix}
$$

follows by induction: multiplying the formula for $n-1$ by $A_n$ gives the two stated recurrences in the first column and $b_n(p_{n-1},q_{n-1})^T$ in the second. The associated Möbius transformations $z\mapsto a_j+b_j/z$, applied from the right to $a_n$, show that the first-column ratio is the displayed [positive generalized continued fraction](../../../../../positive-generalized-continued-fraction.md).

Now set every $b_j=1$. Taking [determinants](../../../../../determinant.md) in the [matrix](../../../../../matrix.md) identity gives

$$
p_nq_{n-1}-q_np_{n-1}=(-1)^{n+1}.
$$

Consequently adjacent convergents differ by

$$
\frac{p_{n+1}}{q_{n+1}}-\frac{p_n}{q_n}
=\frac{(-1)^{n+2}}{q_nq_{n+1}}.
$$

The recurrence and $a_j\geq1$ imply $q_{n+1}\geq q_n+q_{n-1}$, so $q_n\to\infty$. The [determinant](../../../../../determinant.md) signs show that the even convergents increase, the odd convergents decrease, and every even one is below every odd one. Their adjacent separation tends to zero, so both subsequences have a common [limit](../../../../../limit-of-a-function.md) $x$. Since $x$ lies between each adjacent pair, the [convergence of a positive simple continued fraction](../../../../../convergence-of-a-positive-simple-continued-fraction.md) gives exactly

$$
\left|\frac{p_n}{q_n}-x\right|
+\left|\frac{p_{n+1}}{q_{n+1}}-x\right|
=\frac1{q_nq_{n+1}}.
$$

If all $a_j=1$ as well, the recurrence and initial values give

$$
p_n=F_{n+2},\qquad q_n=F_{n+1}.
$$

The characteristic roots of $F_{n+2}=F_{n+1}+F_n$ are  
$\phi=(1+\sqrt5)/2$ and $\psi=(1-\sqrt5)/2=-\phi^{-1}$, hence

$$
F_n=\frac{\phi^n-\psi^n}{\sqrt5}.
$$

Therefore $F_{n+2}/F_{n+1}\to\phi$. Moreover,

$$
F_{n+1}-\phi F_n=\psi^n,\qquad
F_{n+2}-\phi F_{n+1}=\psi^{n+1}.
$$

Using $F_n\phi^{-n}\to1/\sqrt5$ yields

$$
F_nF_{n+1}\left|\frac{F_{n+1}}{F_n}-\phi\right|
=F_{n+1}\phi^{-n}\longrightarrow\frac{\phi}{\sqrt5},
$$

and

$$
F_nF_{n+1}\left|\frac{F_{n+2}}{F_{n+1}}-\phi\right|
=F_n\phi^{-(n+1)}\longrightarrow\frac1{\phi\sqrt5}.
$$

This is the [all-one continued fraction and Fibonacci ratios](../../../../../all-one-continued-fraction-and-fibonacci-ratios.md) case.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
