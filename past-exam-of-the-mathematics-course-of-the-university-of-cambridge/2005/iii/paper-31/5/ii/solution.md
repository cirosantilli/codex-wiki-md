<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $t=\sqrt{-30}$ and $K=\mathbb Q(t)$. The [ring of integers](../../../../../../ring-of-integers.md) is $\mathbb Z[t]$, and the [fundamental discriminant](../../../../../../fundamental-discriminant.md) is $D_K=-120$. For a [reduced positive definite binary quadratic form](../../../../../../reduced-positive-definite-binary-quadratic-form.md) $(a,b,c)$ of discriminant $-120$, reduction gives

$$
|b|\leq a\leq c,\qquad b^2-4ac=-120,\qquad
1\leq a\leq\sqrt{120/3}<7.
$$

The coefficient $b$ is even; checking $1\leq a\leq6$ and $|b|\leq a$, with the usual nonnegative sign choice at boundary equalities, leaves precisely

$$
(1,0,30),\quad(2,0,15),\quad(3,0,10),\quad(5,0,6).
$$

The correspondence between proper quadratic forms and [ideal classes](../../../../../../ideal-class.md) therefore gives $h_K=4$. All four classes equal their inverses, since inversion replaces $b$ by $-b$. Hence

$$
\operatorname{Cl}(K)\cong C_2\times C_2.
$$

The three nontrivial classes may be represented by the ramified [prime ideals](../../../../../../prime-ideal.md) $\mathfrak p_2=(2,t)$, $\mathfrak p_3=(3,t)$ and $\mathfrak p_5=(5,t)$. They square to [principal ideals](../../../../../../principal-ideal.md) and satisfy $\mathfrak p_2\mathfrak p_3\mathfrak p_5=(t)$. None is principal: an integral generator of norm $2$, $3$ or $5$ would require $a^2+30b^2$ to equal that number, which is impossible. The relation then makes the three classes distinct, consistently with the four-form calculation.

Consider

$$
H=\mathbb Q(\sqrt2,\sqrt{-3},\sqrt5).
$$

The three rational [square classes](../../../../../../square-class.md) are independent, so $[H:\mathbb Q]=8$. Their radical product is $\sqrt{-30}$, so $K\subset H$ and $[H:K]=4$; the extension $H/K$ is abelian. To verify that it is unramified, rather than assuming that radical adjunctions are harmless at $2,3,5$, use the [conductor-discriminant formula](../../../../../../conductor-discriminant-formula.md). The seven quadratic subfields have [fundamental discriminants](../../../../../../fundamental-discriminant.md)

$$
8,\ -3,\ 5,\ -24,\ 40,\ -15,\ -120.
$$

The formula gives

$$
|D_H|=8\cdot3\cdot5\cdot24\cdot40\cdot15\cdot120=120^4.
$$

The discriminant tower identity now gives

$$
|D_H|=|D_K|^{[H:K]}N_{K/\mathbb Q}(\mathfrak d_{H/K}),\qquad
N_{K/\mathbb Q}(\mathfrak d_{H/K})=1.
$$

Thus the [relative discriminant](../../../../../../relative-discriminant.md) is the [unit ideal](../../../../../../unit-ideal.md) and no finite prime ramifies. The base has no real places, so there is no infinite ramification to check. This unramified abelian degree-four extension has degree $h_K$, and part (i) proves

$$
\boxed{H_K=\mathbb Q(\sqrt2,\sqrt{-3},\sqrt5).}
$$

This is the [Hilbert class field of Q of square root minus thirty](../../../../../../hilbert-class-field-of-q-of-square-root-minus-thirty.md).

Next translate prime representation into an [ideal class](../../../../../../ideal-class.md). For $p\nmid30$, we claim

$$
p=2x^2+15y^2\text{ for integers }x,y
\quad\Longleftrightarrow\quad
\text{some prime }\mathfrak P\text{ of norm }p\text{ has }[\mathfrak P]=[\mathfrak p_2].
$$

If a representation exists, $\alpha=2x+yt$ lies in $\mathfrak p_2$ and has $N_{K/\mathbb Q}\alpha=2p$. The [integral ideal](../../../../../../integral-ideal.md) $(\alpha)\mathfrak p_2^{-1}$ has norm $p$, so it is a [prime ideal](../../../../../../prime-ideal.md) $\mathfrak P$. Its class is $[\mathfrak p_2]^{-1}=[\mathfrak p_2]$. Conversely, if $[\mathfrak P]=[\mathfrak p_2]$, the product $\mathfrak p_2\mathfrak P$ is principal, say $(\alpha)$. Since this [ideal](../../../../../../ideal.md) lies in $\mathfrak p_2$, its generator has the form $\alpha=2x+yt$ with [integers](../../../../../../integer.md) $x,y$. Taking norms gives $4x^2+30y^2=2p$, proving the reverse implication. This is [prime representation via an ideal class](../../../../../../prime-representation-via-an-ideal-class.md), and it proves sufficiency as well as necessity.

Identify the required class in $\operatorname{Gal}(H/K)$ through the [Artin map](../../../../../../artin-reciprocity-law.md). We can use the explicit representation $17=2+15$: $2+t$ has norm $34$, so the prime above $17$ obtained from $(2+t)\mathfrak p_2^{-1}$ has class $[\mathfrak p_2]$. Its Frobenius in the multiquadratic extension acts on the three radicals with signs

$$
\left(\left(\frac2{17}\right),\left(\frac{-3}{17}\right),\left(\frac5{17}\right)\right)=(1,-1,-1).
$$

Their product is one, so this [automorphism](../../../../../../automorphism.md) fixes $K$. Because $H/\mathbb Q$ is abelian, for any unramified rational prime $p$ that splits in $K$, the Frobenius at either prime of $K$ of norm $p$ is its rational Frobenius restricted to $H/K$. The Artin [isomorphism](../../../../../../isomorphism.md) therefore makes the required class condition equivalent to

$$
\left(\frac2p\right)=1,\qquad
\left(\frac{-3}p\right)=-1,\qquad
\left(\frac5p\right)=-1.
$$

Conversely, these signs already imply splitting in $K$, since their product is $(\frac{-30}p)=1$. No extra splitting condition is missing.

The supplementary law for $2$, [quadratic reciprocity](../../../../../../quadratic-reciprocity.md) for $-3$ and $5$, and then the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) turn these sign conditions into

$$
p\equiv1\text{ or }7\pmod8,\qquad
p\equiv2\pmod3,\qquad
p\equiv2\text{ or }3\pmod5.
$$

Their four simultaneous [residue classes](../../../../../../residue-class.md) modulo $120$ are $17,23,47,113$. Finally, $2$ is represented by $(x,y)=(\pm1,0)$, whereas $3$ and $5$ cannot be represented: $y\ne0$ gives a value at least $15$, and $y=0$ gives twice a square. We have proved the complete criterion

$$
\boxed{p=2x^2+15y^2\text{ is soluble}\iff
p=2\text{ or }p\equiv17,23,47,113\pmod{120}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
