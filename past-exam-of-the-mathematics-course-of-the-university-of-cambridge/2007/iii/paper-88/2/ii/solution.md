<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Freiman 2-isomorphism](../../../../../../freiman-2-isomorphism.md) is an [injective](../../../../../../injective-function.md) map onto its image preserving pair-sum equality in both directions, with repeated summands allowed. Put $D=2A-2A$, so $D=-D$, $0\in D$, and $|D|<N$. We prove the [half-size cyclic Freiman model with a sharp difference-set bound](../../../../../../half-size-cyclic-freiman-model-with-a-sharp-difference-set-bound.md). Assume $A\ne\varnothing$; for an empty [set](../../../../../../set-split.md) the conclusion is immediate.

Choose an odd auxiliary [prime](../../../../../../prime-number.md) $P>N$ large enough that reduction modulo $P$ is [injective](../../../../../../injective-function.md) on $A$ and no nonzero element of $D$ reduces to zero. Choose a multiplier $t$ uniformly in $\mathbb Z_P^\times$. The forbidden residues are

$$
\mathcal F=\{jN\pmod P: j\in\mathbb Z,\ 0<|jN|<P\}.
$$

They form a symmetric [set](../../../../../../set-split.md), exclude zero since $P>N$, and have [cardinality](../../../../../../cardinality.md) at most $2\lfloor(P-1)/N\rfloor$. For each nonzero $d\in D$, the product $td$ is uniform on the $P-1$ nonzero residues. Moreover, $td\in\mathcal F$ is the same event as $t(-d)\in\mathcal F$, so one need only sum over the $(|D|-1)/2$ opposite pairs. The [union bound](../../../../../../boole-s-inequality.md) gives

$$
\Pr\bigl(td\in\mathcal F\text{ for some }d\in D\setminus\{0\}\bigr)\leq\frac{|D|-1}{2}\frac{2\lfloor(P-1)/N\rfloor}{P-1}\leq\frac{|D|-1}{N}<1.
$$

Fix a multiplier avoiding all forbidden events. The use of opposite pairs is what achieves the threshold $N>|D|$ without an extra factor of two.

Represent each $ta\pmod P$ by an [integer](../../../../../../integer.md) $r(a)\in\{0,\ldots,P-1\}$. Partition these residues into the two half-intervals

$$
I_0=\{0,\ldots,(P-1)/2\},\qquad I_1=\{(P+1)/2,\ldots,P-1\}.
$$

At least half of $A$ has representatives in one of them; call this [subset](../../../../../../subset.md) $A'$. Both intervals have diameter less than $P/2$, so for $a_1,a_2,a_3,a_4\in A'$ the [integer](../../../../../../integer.md)

$$
R=r(a_1)+r(a_2)-r(a_3)-r(a_4)
$$

satisfies $|R|<P$.

Define $\phi(a)=r(a)\pmod N$. If $a_1+a_2=a_3+a_4$, then $R\equiv0\pmod P$, hence $R=0$ and the image relation holds. Conversely, if the image relation holds, then $R=jN$. If the original difference $d=a_1+a_2-a_3-a_4$ were nonzero, $R\equiv td\pmod P$ would be nonzero; since $|R|<P$, this would be a forbidden residue in $\mathcal F$. Thus $d=0$.

Finally $\phi$ is [injective](../../../../../../injective-function.md). If $\phi(a)=\phi(b)$, choose any $c\in A'$ and apply the converse to $\phi(a)+\phi(c)=\phi(b)+\phi(c)$, obtaining $a+c=b+c$. Therefore

$$
\boxed{|A'|\geq|A|/2,\qquad\phi:A'\longrightarrow\phi(A')\subseteq\mathbb Z_N\text{ is a Freiman 2-isomorphism}.}
$$

The construction actually works for any [integer](../../../../../../integer.md) $N>|D|$; the [prime](../../../../../../prime-number.md) hypothesis in the question is sufficient.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
