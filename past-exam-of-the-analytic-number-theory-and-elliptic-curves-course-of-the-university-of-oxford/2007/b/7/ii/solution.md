<h1 id="b/7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an affine point of $C$ with $x\ne0$, the first coordinate of its image is $(y/x)^2$. Thus its image has trivial [square class](../../../../../square-class.md) whenever that coordinate is nonzero. The identity and $T=(0,0)$ map to the identity. If a point maps to $T_1=(0,0)$, it has $y=0$ and $x^2+ax+b=0$, forcing $b_1=a^2-4b$ to be a rational square; in that case $q(T_1)=1$ too. Hence $\phi(C(\mathbb Q))\subseteq\ker q$.

Conversely, let $(u,v)\in D(\mathbb Q)$ have $q(u,v)=1$ and $u\ne0$. Write $u=t^2$ with $t\in\mathbb Q^*$. The equation of $D$ gives

$$
(v/t)^2=(u-a)^2-4b.
$$

Set $x=(u-a+v/t)/2$ and $y=tx$. Then $x$ solves $x^2+(a-u)x+b=0$ and is nonzero because $b\ne0$. Hence $y^2=ux^2=x(x^2+ax+b)$, so $(x,y)\in C(\mathbb Q)$. Also $x-b/x=v/t$, giving $\phi(x,y)=(u,v)$.

The identity is an image of the identity. Finally, $T_1\in\ker q$ exactly when $b_1$ is a rational square; then either nonzero root $x=(-a\pm\sqrt{b_1})/2$ gives $(x,0)\in C(\mathbb Q)$ mapping to $T_1$. This covers all exceptional points and proves

$$
\boxed{\ker q=\phi(C(\mathbb Q)).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
