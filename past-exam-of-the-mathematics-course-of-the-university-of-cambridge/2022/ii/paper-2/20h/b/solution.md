<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dedekind factorization theorem](../../../../../../dedekind-factorization-theorem.md) says that, when a rational prime $p$ does not divide the index of an order $\mathbb Z[\theta]\subseteq\mathcal O_K$, a factorization

$$
\overline f=\prod_i\overline g_i^{e_i}
$$

of the [minimal polynomial](../../../../../../minimal-polynomial.md) modulo $p$ gives

$$
p\mathcal O_K=\prod_i(p,g_i(\theta))^{e_i}.
$$

Let $K=\mathbb Q(\sqrt d)$ with square-free $d$, and let $p$ be odd. The resulting [splitting of rational primes in a quadratic field](../../../../../../splitting-of-rational-primes-in-a-quadratic-field.md) is:

$$
\begin{array}{c|c}
p\mid d & (p)=P^2\quad\text{(ramified)},\\
\left(\frac dp\right)=1 &(p)=(p,\sqrt d-a)(p,\sqrt d+a),
\quad a^2\equiv d\pmod p,\\
\left(\frac dp\right)=-1 &(p)\ \text{is prime}.
\end{array}
$$

Finally suppose $d>0$ and  
$\alpha=A/C+(B/C)\sqrt d$ has norm $-1$, with integers  
$A,B,C$ chosen [coprime](../../../../../../coprime-integers.md). Then

$$
A^2-dB^2=-C^2.
$$

If an [odd](../../../../../../odd-integer.md) $p\equiv3\pmod4$ [ramified](../../../../../../ramification-of-a-prime.md), then $p\mid d$. [Reduction](../../../../../../reduction-modulo-an-ideal.md) modulo $p$ gives  
$A^2\equiv-C^2\pmod p$. Since $-1$ is not a [square](../../../../../../quadratic-residue.md) modulo such a [prime](../../../../../../prime-number.md), $p\mid A,C$. Dividing the equation's [divisibility](../../../../../../divisibility.md) shows $p\mid B$ as well (use that [square-free](../../../../../../square-free-integer.md) $d$ has [$p$-adic valuation](../../../../../../p-adic-valuation.md) one), contradicting [coprimality](../../../../../../coprime-integers.md). Hence no prime $p\equiv3\pmod4$ ramifies.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
