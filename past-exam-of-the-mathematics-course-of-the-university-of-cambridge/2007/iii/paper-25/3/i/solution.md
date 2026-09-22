<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the square as $GH=KF$, with $F:\mathcal A\to\mathcal B$ final and $G:\mathcal C\to\mathcal D$ a [discrete fibration](../../../../../../discrete-fibration.md). For $b\in\mathcal B$, choose an object $(a,h:b\to Fa)$ of the nonempty [comma category](../../../../../../comma-category.md) $(b\downarrow F)$. Lift $K(h):Kb\to GHa$ uniquely to an arrow

$$
\ell_h:c_h\longrightarrow Ha
$$

over $K(h)$, and tentatively put $L(b)=c_h$.

A morphism $(a,h)\to(a',h')$ in this [comma category](../../../../../../comma-category.md) is an arrow $j:a\to a'$ with $F(j)h=h'$. The composite $H(j)\ell_h$ is a lift of $K(h')$ with codomain $Ha'$. Uniqueness of lifts gives $H(j)\ell_h=\ell_{h'}$, including equality of their source objects. Since the [comma category](../../../../../../comma-category.md) is connected by zigzags, $c_h$ is independent of the choice. Thus $L(b)$ is well defined and $GL(b)=Kb$.

For $f:b\to b'$, take $(a',h':b'\to Fa')$. Lift $K(f)$ into $L(b')$, obtaining $t:c\to L(b')$. Composing with $\ell_{h'}$ gives a lift of $K(h'f)$ into $Ha'$, whose source must be $L(b)$. Hence $t:L(b)\to L(b')$. Set $L(f)=t$. Uniqueness of this lift makes the definition independent of the chosen comma object and proves $L(1_b)=1_{L(b)}$ and $L(gf)=L(g)L(f)$.

At $b=Fa$, choose $(a,1_{Fa})$. Its lift is $1_{Ha}$, so $L(Fa)=Ha$. For $j:a\to a'$, $Hj$ is the unique lift of $K(Fj)$ into $Ha'$, so $L(Fj)=Hj$. We have constructed the required [functor](../../../../../../functor.md) with $LF=H$ and $GL=K$.

If $L'$ is another filler, $L'(h):L'b\to Ha$ must equal $\ell_h$ by unique lifting. Thus $L'b=L(b)$ for every object. Its arrows are then forced by unique lifting into those objects. Therefore

$$
\boxed{L\text{ exists and is unique}.}
$$

This proves the [orthogonality of final functors and discrete fibrations](../../../../../../orthogonality-of-final-functors-and-discrete-fibrations.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
