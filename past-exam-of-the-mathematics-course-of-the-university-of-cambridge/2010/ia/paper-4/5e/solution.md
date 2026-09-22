<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

For the [Fibonacci addition formula](../../../../../fibonacci-addition-formula.md), use [mathematical induction](../../../../../mathematical-induction.md) on $k$, with the assertion applying to every $n\ge1$. At $k=2$, $F_{n+2}=F_{n+1}+F_n=F_2F_{n+1}+F_1F_n$. If the formula holds for some $k\ge2$ and all $n$, apply it at $n+1$ and use the [Fibonacci number](../../../../../fibonacci-number.md) recurrence:

$$
\begin{aligned}
F_{n+k+1}
&=F_kF_{n+2}+F_{k-1}F_{n+1}\\
&=F_k(F_{n+1}+F_n)+F_{k-1}F_{n+1}\\
&=F_{k+1}F_{n+1}+F_kF_n.
\end{aligned}
$$

This is the assertion at $k+1$, completing the [mathematical induction](../../../../../mathematical-induction.md). Thus

$$
\boxed{F_{n+k}=F_kF_{n+1}+F_{k-1}F_n\quad(n\ge1,\ k\ge2).}
$$

Taking $k=n\ge2$ gives the doubling identity

$$
\boxed{F_{2n}=F_n(F_{n+1}+F_{n-1})=F_nL_n.}
$$

For the [Lucas numbers](../../../../../lucas-number.md), $L_2=F_3+F_1=3$, and $L_3=F_4+F_2=4=L_2+L_1$. For $n\ge4$, both expressions for earlier [Lucas numbers](../../../../../lucas-number.md) are available, and

$$
L_{n-1}+L_{n-2}
=(F_n+F_{n-2})+(F_{n-1}+F_{n-3})
=F_{n+1}+F_{n-1}=L_n.
$$

Hence $\boxed{L_1=1,\quad L_2=3,\quad L_n=L_{n-1}+L_{n-2}\ (n\ge3)}$. The separate $n=3$ check matters because the defining expression for $L_1$ was given separately.

The [Euclidean algorithm](../../../../../euclidean-algorithm.md) and the [Fibonacci number](../../../../../fibonacci-number.md) recurrence give, for $n\ge2$,

$$
\gcd(F_n,F_{n+1})=\gcd(F_n,F_{n-1}).
$$

Repeating reduces to $\gcd(F_2,F_1)=1$; the case $n=1$ is immediate. Therefore $\boxed{\gcd(F_n,F_{n+1})=1\ (n\ge1)}$.

For $n\ge2$, $L_n=F_n+2F_{n-1}$, so a common divisor $d$ of $F_n,L_n$ divides both $F_n$ and $2F_{n-1}$. Since $F_n,F_{n-1}$ are coprime, [Bézout's identity](../../../../../bezout-identity.md) gives integers $s,t$ with $sF_n+tF_{n-1}=1$. Multiplying by $2$ shows $d\mid2$. Conversely any common divisor of $F_n$ and $2$ divides $L_n$. Including $n=1$, this proves the stronger [greatest common divisor](../../../../../greatest-common-divisor.md) identity

$$
\boxed{\gcd(F_n,L_n)=\gcd(F_n,2)\le2\quad(n\ge1).}
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
