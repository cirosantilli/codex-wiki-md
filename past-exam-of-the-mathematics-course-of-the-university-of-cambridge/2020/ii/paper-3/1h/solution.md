<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Put $e=(N-1)/2$. The odd integer $N$ is an [Euler pseudoprime](../../../../../euler-pseudoprime.md) to the [coprime](../../../../../coprime-integers.md) base $b$ when

$$
b^e\equiv\left(\frac bN\right)\pmod N,
$$

where $(b/N)$ is the [Jacobi symbol](../../../../../jacobi-symbol.md).

Let $G=(\mathbb Z/N\mathbb Z)^\times$ be the [unit group](../../../../../unit-group.md) of [residue classes](../../../../../residue-class.md) modulo $N$, and partition it into the set $E$ of bases satisfying the displayed congruence and the set $W$ of [Euler witnesses](../../../../../euler-witness.md) that do not. If $b_0\in W$, multiplication by $b_0$ maps $E$ [injectively](../../../../../injective-function.md) into $W$: indeed, if $b\in E$ and $bb_0$ also lay in $E$, then the [multiplicativity of the Jacobi symbol](../../../../../multiplicativity-of-the-jacobi-symbol.md) would give

$$
b^eb_0^e\equiv\left(\frac bN\right)\left(\frac {b_0}N\right)\pmod N.
$$

Cancelling the invertible congruence for $b$ would say that $b_0\in E$, a contradiction. Hence $|W|\geq |E|$, so at least half of the [coprime](../../../../../coprime-integers.md) bases are witnesses.

It remains to construct one witness for every odd [composite number](../../../../../composite-number.md) $N$. If $N$ is not [squarefree](../../../../../squarefree-integer.md), choose an odd [prime number](../../../../../prime-number.md) $p$ with $p^2\mid N$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives a unit $b$ such that $b\equiv1+p\pmod {p^a}$ for the full power $p^a\mid N$ and $b\equiv1$ modulo every other prime-power factor. The [binomial theorem](../../../../../binomial-theorem.md) gives

$$
b^e\equiv(1+p)^e\equiv1+ep\pmod {p^2}.
$$

Since $p\nmid e$, this is neither $1$ nor $-1$ modulo $p^2$, whereas the [Jacobi symbol](../../../../../jacobi-symbol.md) is always $1$ or $-1$. Thus $b$ is a witness.

If $N$ is squarefree and composite, choose distinct primes $p,q\mid N$. By the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md), choose $b$ to be a [quadratic nonresidue](../../../../../quadratic-nonresidue.md) modulo $p$ and to satisfy $b\equiv1$ modulo every other prime divisor of $N$. Then $(b/N)=-1$, while $b^e\equiv1\pmod q$, so the Euler congruence again fails. This proves the [existence of an Euler witness for every odd composite integer](../../../../../existence-of-an-euler-witness-for-every-odd-composite-integer.md).

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
