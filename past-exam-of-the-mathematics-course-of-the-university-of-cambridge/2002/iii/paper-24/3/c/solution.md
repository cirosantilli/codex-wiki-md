<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is $37$, so the [elliptic curve](../../../../../../elliptic-curve.md) has [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) at both $2$ and $3$. At a prime $\ell$ of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), the [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) is injective on torsion of order prime to $\ell$. Here is the formal reason: the [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md) is described by an integral [formal group law](../../../../../../formal-group-law.md) on $\ell\mathbb Z_\ell$, and its multiplication series is $[n](t)=nt+O(t^2)$. If $\ell\nmid n$, the first term has strictly smaller [valuation](../../../../../../valuation.md) than every higher term for $t\ne0$. Thus this kernel has no nonidentity point killed by $n$.

Apply this to each prime-primary component of the rational [torsion subgroup](../../../../../../torsion-subgroup.md). A component at $2$ injects into $\widetilde E_3(\mathbb F_3)$, of order $7$, and is therefore trivial. A component at $3$ injects into $\widetilde E_2(\mathbb F_2)$, of order $5$, and is trivial. Every other prime-primary component injects into both groups, so its order divides $\gcd(5,7)=1$. This proves the [two-prime bound on rational elliptic torsion](../../../../../../two-prime-bound-on-rational-elliptic-torsion.md) in the present case:

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{O\}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
