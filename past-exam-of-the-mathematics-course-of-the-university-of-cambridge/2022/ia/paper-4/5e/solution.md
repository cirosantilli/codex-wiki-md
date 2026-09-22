<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

The [Bezout identity](../../../../../bezout-identity.md) states that for integers $a,b$, not both zero, there are integers $r,s$ such that

$$
ra+sb=\gcd(a,b).
$$

If the [prime number](../../../../../prime-number.md) $p$ divides $ab$ but does not divide $a$, then $\gcd(p,a)=1$. Thus $rp+sa=1$ for some integers $r,s$, and multiplication by $b$ gives

$$
b=rpb+sab.
$$

Both terms on the right are divisible by $p$, so $p\mid b$. Hence

$$
\boxed{p\mid ab\Longrightarrow p\mid a\text{ or }p\mid b}.
$$

If $\gcd(m,n)=1$, choose $r,s$ with $rm+sn=1$. Then

$$
x=a(sn)+b(rm)
$$

satisfies $x\equiv a\pmod m$ and $x\equiv b\pmod n$. If $x,x'$ are two simultaneous solutions, both $m$ and $n$ divide $x-x'$. Coprimality implies $mn\mid x-x'$, so the solution is unique modulo $mn$. This proves the two-modulus [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md).

Let $p$ be odd and suppose

$$
x^2\equiv1\pmod{p^d}.
$$

Then $p^d\mid(x-1)(x+1)$. Since $\gcd(x-1,x+1)$ divides $2$, the odd prime $p$ cannot divide both factors. The full power $p^d$ must therefore divide one of them, giving

$$
x\equiv1\pmod{p^d}
\quad\hbox{or}\quad
x\equiv-1\pmod{p^d}.
$$

These are distinct, so there are exactly two solutions.

For an odd integer

$$
n=\prod_{j=1}^kp_j^{d_j},
$$

the Chinese remainder theorem identifies a solution modulo $n$ with independent solutions modulo the $k$ [prime powers](../../../../../prime-power.md). Each component has two choices, hence

$$
\boxed{\#\{x\bmod n:x^2\equiv1\}=2^k}.
$$

For $n=2^d$, there is one solution when $d=1$ and two when $d=2$. If $d\geq3$, a solution $x$ is odd, and of the consecutive even integers $x-1,x+1$, exactly one is divisible by $4$. The [2-adic valuations](../../../../../p-adic-valuation.md) therefore have minimum one; for their sum to be at least $d$, the other must be at least $d-1$. Thus $x\equiv\pm1\pmod{2^{d-1}}$, giving the four distinct classes

$$
1,\quad -1,\quad1+2^{d-1},\quad-1+2^{d-1}\pmod{2^d}.
$$

Consequently the answer is

$$
\boxed{
\begin{cases}
1,&d=1,\\
2,&d=2,\\
4,&d\geq3.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
