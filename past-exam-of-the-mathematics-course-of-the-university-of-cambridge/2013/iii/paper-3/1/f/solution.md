<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the [Sylow theorems](../../../../../../sylow-theorems.md). The number $n_p$ divides $qr$ and is congruent to one modulo $p$. Since $q,r<p$, it is either one or $qr$. Suppose $n_p=qr$. Different subgroups of prime order intersect trivially, so their nonidentity elements occupy $qr(p-1)$ places, leaving only $qr-1$ nonidentity elements of other prime orders.

If neither the Sylow $q$-subgroup nor the Sylow $r$-subgroup is normal, then $n_q\geq p$ and $n_r\geq q$. Indeed $n_q$ divides $pr$, and its possible divisor $r<q$ cannot satisfy the Sylow congruence; the smallest remaining nontrivial possibility is at least $p$. Likewise any nontrivial divisor of $pq$ is at least $q$. Their elements would require at least

$$
p(q-1)+q(r-1)>qr-1
$$

places, since the excess is $(p-1)(q-1)>0$. Hence some [Sylow subgroup](../../../../../../sylow-subgroup.md) of order $s\in\{q,r\}$ is normal.

In the quotient by this [normal subgroup](../../../../../../normal-subgroup.md), the largest prime $p$ has a normal [Sylow subgroup](../../../../../../sylow-subgroup.md): for a group of order $pt$ with $p>t$ its Sylow count divides $t<p$ and so equals one. Pulling back gives a [normal subgroup](../../../../../../normal-subgroup.md) of order $ps$. Inside it, the subgroup of order $p$ is again the unique Sylow $p$-subgroup. It is characteristic in that [normal subgroup](../../../../../../normal-subgroup.md) and therefore normal in $G$, contradicting $n_p=qr$. Thus $\boxed{n_p=1}$.

Let $P$ be this normal [Sylow subgroup](../../../../../../sylow-subgroup.md). In $G/P$, of order $qr$, its subgroup of order $q$ is normal by the same argument. Its preimage $K$ is a **normal Hall $\{p,q\}$-subgroup**. The series

$$
1\lhd P\lhd K\lhd G
$$

has factors of orders $p,q,r$, hence cyclic and abelian. Therefore $\boxed{G\text{ is soluble}.}$ This establishes solubility before using any Hall-existence conclusion that itself assumes solubility.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
