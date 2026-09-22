<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The [Euclidean algorithm](../../../../../euclidean-algorithm.md) and the [Fibonacci number](../../../../../fibonacci-number.md) recurrence give

$$
\gcd(F_{n+1},F_n)=\gcd(F_n,F_{n+1}-F_n)=\gcd(F_n,F_{n-1}).
$$

Iterating reaches $\gcd(F_1,F_0)=\gcd(1,0)=1$, so **consecutive Fibonacci numbers are coprime**.

Prove the [Fibonacci addition formula](../../../../../fibonacci-addition-formula.md) by [mathematical induction](../../../../../mathematical-induction.md) on $k$, asserting it simultaneously for every $n\ge0$. At $k=1$, $F_1F_{n+1}+F_0F_n=F_{n+1}$. Suppose the formula holds at $k$. Apply it with $n+1$ in place of $n$ and use the recurrence:

$$
\begin{aligned}
F_{n+k+1}&=F_kF_{n+2}+F_{k-1}F_{n+1}\\
&=(F_k+F_{k-1})F_{n+1}+F_kF_n\\
&=F_{k+1}F_{n+1}+F_kF_n.
\end{aligned}
$$

Thus

$$
\boxed{F_{n+k}=F_kF_{n+1}+F_{k-1}F_n\qquad(n\ge0,\ k\ge1).}
$$

For $n\ge1$, prove $F_n\mid F_{nl}$ by induction on $l$. The case $l=1$ is immediate. For $l\ge2$, put $k=(l-1)n$ in the addition formula. Its first term is divisible by $F_n$ by the induction hypothesis, and its second term has an explicit factor $F_n$. Therefore

$$
\boxed{F_n\mid F_{nl}\qquad(l\ge1).}
$$

When $m>n\ge1$, put $k=m-n$. Reducing the addition formula modulo $F_n$ gives $F_m\equiv F_{m-n}F_{n+1}$. Since $F_{n+1}$ is coprime to $F_n$, multiplication by it leaves the [greatest common divisor](../../../../../greatest-common-divisor.md) with $F_n$ unchanged: any divisor of $F_n$ dividing the product divides $F_{m-n}$, by the [Bezout identity](../../../../../bezout-identity.md) or the [Euclid lemma](../../../../../euclid-lemma.md). This proves the [Fibonacci gcd reduction](../../../../../fibonacci-gcd-reduction.md)

$$
\boxed{\gcd(F_m,F_n)=\gcd(F_{m-n},F_n)\qquad(m\ge n).}
$$

At $m=n$ both sides equal $F_n$, since $F_0=0$. The case $n=0$ is also immediate from $\gcd(a,0)=|a|$; the divisibility statement at $n=0$ reads $0\mid0$, valid under the usual definition $b\mid a$ iff $a=bc$ for an integer $c$.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
