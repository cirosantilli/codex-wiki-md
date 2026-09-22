<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since neither $n$ nor $-n$ is a square, both cubics have exactly one rational root, zero. Thus each [torsion point of an elliptic curve](../../../../../torsion-point-of-an-elliptic-curve.md) [group](../../../../../group-split.md) has exactly one nonidentity [2-torsion](../../../../../2-torsion.md), namely $T=(0,0)$.

Neither curve has a [rational point](../../../../../rational-point.md) of order four. Indeed on $E_m:y^2=x^3+mx$ the duplication formula gives

$$
x(2P)=\frac{(x(P)^2-m)^2}{4y(P)^2}.
$$

If $2P=T$, then $P$ is neither the identity nor a [2-torsion](../../../../../2-torsion.md), so the denominator is nonzero and $x(P)^2=m$. Thus $m$ must be a rational square; an [integer](../../../../../integer-split.md) that is a rational square is an [integer](../../../../../integer-split.md) square. Applying this with $m=n$ or $m=-n$ contradicts the hypotheses.

If $3\nmid n$, both curves have [good reduction of an elliptic curve](../../../../../good-reduction-of-an-elliptic-curve.md) at three and exactly four points over $\mathbb F_3$. To see this, $x^3=x$ there, so the equation is $y^2=(1+m)x$. For $m=1$ the right side runs through all [residues](../../../../../residue.md), and for $m=-1$ it is always zero; either way there are three affine points. Injection of [torsion point of an elliptic curve](../../../../../torsion-point-of-an-elliptic-curve.md) at this odd good [prime](../../../../../prime-number-split.md) bounds each [torsion element](../../../../../torsion-element.md) order by four. An order-four [torsion subgroup](../../../../../torsion-subgroup.md) with just one nonzero [2-torsion](../../../../../2-torsion.md) would contain an order-four point, which was excluded. Therefore in this case both [torsion subgroups](../../../../../torsion-subgroup.md) equal $\{o,T\}$.

The remaining case is $3\mid n$. The literal hypothesis $15\nmid n$ then ensures $5\nmid n$, so both curves have [good reduction of an elliptic curve](../../../../../good-reduction-of-an-elliptic-curve.md) at five. Direct square counting gives

$$
\begin{array}{c|rrrr}
m\bmod5&1&2&3&4\\\hline
\#E_m(\mathbb F_5)&4&2&10&8.
\end{array}
$$

For example the square [residues](../../../../../residue.md) are $0,1,4$; substituting $x=0,\ldots,4$ gives this table, including the point at infinity. The pair $m=n,-n$ has [residues](../../../../../residue.md) $(1,4)$ or $(2,3)$ in some order. In either pair at least one reduction [group](../../../../../group-split.md) has order two or four. The same injection and absence of order-four points then force that curve's [torsion point of an elliptic curve](../../../../../torsion-point-of-an-elliptic-curve.md) to have order two. Thus

$$
\boxed{\text{at least one of }E(\mathbb Q)_{\rm tors},
F(\mathbb Q)_{\rm tors}\text{ is }\{o,(0,0)\}.}
$$

This [torsion alternative for opposite quartic-twist coefficients](../../../../../torsion-alternative-for-opposite-quartic-twist-coefficients.md) uses only $15\nmid n$; it does not strengthen the source hypothesis to coprimality with fifteen.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
