<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [orthogonality of final functors and discrete fibrations](../../../../../../orthogonality-of-final-functors-and-discrete-fibrations.md). For $b\in\mathcal B$, [finality](../../../../../../finality-of-a-functor.md) supplies an object $(a,u:b\to Fa)$ of $(b\downarrow F)$. Lift $Ku:Kb\to GHa$ through the [discrete fibration](../../../../../../discrete-fibration.md) $G$, obtaining

$$
j_{a,u}:c_{a,u}\longrightarrow Ha,\qquad Gj_{a,u}=Ku,\qquad Gc_{a,u}=Kb.
$$

If $v:(a,u)\to(a',u')$ in the [comma category](../../../../../../comma-category.md), then $Fv\,u=u'$, and $Hv\,j_{a,u}$ is a lift of $Ku'$ with codomain $Ha'$. Uniqueness of that lift makes its domain equal to $c_{a',u'}$. Thus $c_{a,u}=c_{a',u'}$; since the comma category is a [connected category](../../../../../../connected-category.md), equality propagates along every zigzag. Define $Lb$ to be this common object.

For $w:b\to b'$, choose $(a,u:b'\to Fa)$. Lift $Kw$ into $Lb'$, obtaining $\ell:c\to Lb'$. Then $j_{a,u}\ell$ lifts $K(uw)$ into $Ha$, so its domain is $Lb$ by the preceding construction. Define $Lw=\ell$. The [unique lifting property of a discrete fibration](../../../../../../unique-lifting-property-of-a-discrete-fibration.md) proves $L(1_b)=1_{Lb}$ and $L(w'w)=L(w')L(w)$, and gives $GL=K$.

At $b=Fa$, use $(a,1_{Fa})$; its lift is $1_{Ha}$, so $LFa=Ha$. Both $L(Fv)$ and $Hv$ are lifts of $GHv$ with the same codomain, hence agree. Therefore $LF=H$.

If $L'$ is another filling [functor](../../../../../../functor.md), its arrow $L'u:L'b\to Ha$ is the same unique lift of $Ku$, forcing $L'b=Lb$. Its arrows are likewise forced by their codomains and images under $G$. **The diagonal functor exists and is unique.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [3](../../3.md)
3. [Section B](../../section-b.md)
4. [Paper 23](../../../paper-23-split.md)
5. [Iii](../../../split.md)
6. [2004](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
