<h1 id="5/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Orient the two components coherently through the twist region and assign meridian variables $x,y$. The [link diagram](../../../../../../link-diagram.md) is the [torus link](../../../../../../torus-link.md) $T_{2,2n}$. It is obtained from the three-component [torus link](../../../../../../torus-link.md) of part 2 by $-1/(n-1)$ [rational Dehn surgery](../../../../../../rational-dehn-surgery.md) on the third component: removing its meridional disk adds $n-1$ full twists to the original single full twist. For $n=1$, this just means meridionally deleting the third component.

Write $z$ for the removed component's meridian. Its longitude is homologous to $\mu_1+\mu_2$, so the filling imposes $z=(xy)^{n-1}$. Under this substitution, the polynomial of part 2 becomes $(xy)^n-1$. The filling core is homologous, up to sign, to $\mu_1+\mu_2$. The [Turaev-torsion Dehn-filling formula](../../../../../../turaev-torsion-dehn-filling-formula.md) therefore removes the factor $xy-1$, giving

$$
\boxed{\Delta_{L(n)}(x,y)\doteq\frac{(xy)^n-1}{xy-1}.}
$$

For positive $n$ this is the [Laurent polynomial](../../../../../../laurent-polynomial.md) $1+xy+\cdots+(xy)^{n-1}$. For $n=1$ it is one, as for a [Hopf link](../../../../../../hopf-link.md); for $n=0$ it is zero, as for the two-component [unlink](../../../../../../unlink.md). For negative $n$ the displayed quotient is still a [Laurent polynomial](../../../../../../laurent-polynomial.md) and agrees with the mirrored positive-twist answer up to a unit. These checks also fix the twist count: the exponent is $n$, rather than $n+1$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
