<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the printed bilinear pairing $\phi_u(v)=\int uv$, which is complex linear in both arguments. For the [conjugate exponents](../../../../../../conjugate-exponents.md) $p,q$, [Holder inequality](../../../../../../holder-inequality.md) gives $|\phi_u(v)|\leq\|u\|_q\|v\|_p$, proving well-definedness, continuity, and $\|\phi_u\|\leq\|u\|_q$. Linearity of $u\mapsto\phi_u$ follows from linearity of integration.

For $u\ne0$, take

$$
v=\frac{\overline u\,|u|^{q-2}}{\|u\|_q^{q-1}},
$$

with the numerator defined as zero where $u=0$. Since $(q-1)p=q$, this has $\|v\|_p=1$ and $\phi_u(v)=\|u\|_q$. Hence $\boxed{\|\phi_u\|=\|u\|_q}$; the same identity holds for $u=0$. This also proves injectivity.

For surjectivity, let $\Lambda$ be a nonzero bounded [linear functional](../../../../../../linear-functional.md) on $L^p$. Choose $f$ with $\Lambda(f)=1$ and let $K=\ker\Lambda$. The [closest point theorem for a closed convex subset of Lp](../../../../../../closest-point-theorem-for-a-closed-convex-subset-of-lp.md) supplies the nearest point $h\in K$; write $w=f-h\ne0$. For every $z\in K$, the whole line $h+tz$ lies in $K$, so the norm derivative at the minimum vanishes for real $t$. Applying this also to $iz$ shows that the complex linear functional

$$
\Psi(v)=\int |w|^{p-2}\overline w\,v
$$

vanishes on $K$. Since $\Lambda(w)=1$, each $v-\Lambda(v)w$ is in $K$, giving $\Psi(v)=\Lambda(v)\Psi(w)$ and $\Psi(w)=\|w\|_p^p$. Therefore

$$
\Lambda(v)=\int u\,v,\qquad
u=\frac{|w|^{p-2}\overline w}{\|w\|_p^p}\in L^q.
$$

Membership follows from $(p-1)q=p$. The zero functional is represented by $u=0$. This proves the asserted [Lp duality](../../../../../../lp-duality-on-an-arbitrary-measure-space.md) isometric isomorphism, including surjectivity, without a separate representation theorem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
