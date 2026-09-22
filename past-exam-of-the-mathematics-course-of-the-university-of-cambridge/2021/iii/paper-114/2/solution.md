<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Writing the [suspension of a topological space](../../../../../suspension-topology.md) as two cones and applying the [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) gives the [reduced homology of a suspension](../../../../../reduced-homology-of-a-suspension.md)

$$
\widetilde H_i(\Sigma X;\mathbb Z)
\cong\widetilde H_{i-1}(X;\mathbb Z).
$$

Thus $H_0(\Sigma X)\cong\mathbb Z$ for nonempty $X$, $H_1(\Sigma X)\cong\widetilde H_0(X)$, and the same shift holds in every higher degree. For a space of finite CW type, the reduced [Euler characteristic](../../../../../euler-characteristic.md) changes sign, so

$$
\chi(\Sigma X)=2-\chi(X),
\qquad
\chi(\Sigma^jX)=1+(-1)^j(\chi(X)-1).
$$

Since $\chi(\mathbb{CP}^2)=3$,

$$
\chi(\Sigma^j\mathbb{CP}^2)=1+2(-1)^j\in\{3,-1\}.
$$

But the [Euler characteristic of a product](../../../../../euler-characteristic-of-a-product.md) satisfies $\chi(A\times A)=\chi(A)^2$, a nonnegative perfect square. Neither $3$ nor $-1$ is such a square, so no $\Sigma^j\mathbb{CP}^2$ is [homotopy equivalent](../../../../../homotopy-inverse.md) to $A\times A$.

A homeomorphism $f:\mathbb R^n\to\mathbb R^n$ is a [proper map](../../../../../proper-map.md), so it extends over the [one-point compactification](../../../../../alexandroff-extension.md) to a homeomorphism $f^+:S^n\to S^n$ fixing infinity. Define

$$
\deg f=\deg f^+,
$$

using the [degree of a continuous mapping](../../../../../degree-of-a-continuous-mapping.md). Since $f^+$ acts invertibly on $H_n(S^n;\mathbb Z)\cong\mathbb Z$, its degree is $\pm1$. Functoriality of induced homology maps gives

$$
\deg(f\circ g)=\deg f\deg g.
$$

For $A\in\operatorname{GL}(n,\mathbb R)$, path connectedness of each determinant-sign component reduces $A$ to the identity when $\det A>0$ and to one coordinate reflection when $\det A<0$. Hence

$$
\deg A=\operatorname{sign}(\det A).
$$

Suppose $h:Y\times Y\to\mathbb R^{2n+1}$ were a homeomorphism, and put $d=2n+1$. Then $Y^4\cong\mathbb R^d\times\mathbb R^d\cong\mathbb R^{2d}$. The square of the cyclic permutation

$$
\sigma(y_1,y_2,y_3,y_4)=(y_4,y_1,y_2,y_3)
$$

interchanges the two $Y^2$ factors. Under $h\times h$, it is conjugate to the linear factor swap $(u,v)\mapsto(v,u)$ on $\mathbb R^d\times\mathbb R^d$, whose determinant has sign $(-1)^{d^2}=-1$. Thus $\deg(\sigma^2)=-1$. On the other hand, multiplicativity gives $\deg(\sigma^2)=(\deg\sigma)^2=1$, a contradiction. Therefore no such $Y$ exists.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
