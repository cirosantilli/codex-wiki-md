<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the square's notation $HF=KG$. For $E\in\mathcal E$, choose $(C,u:E\to GC)$ in the nonempty [connected category](../../../../../../connected-category.md) $(E\downarrow G)$. Lift $Ku:KE\to HFC$ through the [discrete fibration](../../../../../../discrete-fibration.md) $H$, obtaining the uniquely determined arrow

$$
\widetilde u:D_u\longrightarrow FC,\qquad H\widetilde u=Ku.
$$

Define $LE=D_u$. If $a:C\to C'$ satisfies $Ga\,u=u'$, then $Fa\,\widetilde u$ is a lift of $Ku'$ with codomain $FC'$. Uniqueness makes it exactly $\widetilde u'$, including equality of its domain. Connectedness of the [comma category](../../../../../../comma-category.md) therefore makes $LE$ independent of the chosen object, with strict equality rather than merely an isomorphism.

For $v:E\to E'$, choose $(C,u:E'\to GC)$ and lift $Kv:KE\to KE'=HLE'$ with codomain $LE'$. Write this lift as $w:D\to LE'$. Its composite with $\widetilde u$ is the lift of $K(uv)$ to $FC$, so its domain is $LE$. Set $Lv=w$. The lift of an identity is an identity, and the composite of two lifts is the lift of the composite with the specified codomain. Thus $L$ is a [functor](../../../../../../functor.md), and $HL=K$.

At $E=GC$, choose $(C,1_{GC})$; its lift is $1_{FC}$, giving $LGC=FC$. For $a:C\to C'$, the unique lift of $KGa=HFa$ with codomain $FC'$ is $Fa$, giving $LG=F$ on arrows as well. Finally, any other filler $L'$ must send $u$ to the same lift of $Ku$ with codomain $FC$, so $L'E=LE$; it must also send $v$ to the unique lift of $Kv$ with codomain $LE'$. This proves [orthogonality of final functors and discrete fibrations](../../../../../../orthogonality-of-final-functors-and-discrete-fibrations.md):

$$
\boxed{\exists!\,L:\mathcal E\to\mathcal D\text{ with }HL=K,\quad LG=F.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
