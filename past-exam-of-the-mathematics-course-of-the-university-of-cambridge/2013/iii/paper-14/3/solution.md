<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard complex orientations and the product orientation. Let $a,b\in H^2(S^2\times S^2;\mathbb Z)$ satisfy $a^2=b^2=0$ and $\langle ab,[S^2\times S^2]\rangle=1$, and let $x\in H^2(\mathbb{CP}^2;\mathbb Z)$ satisfy $\langle x^2,[\mathbb{CP}^2]\rangle=1$. These are the [cohomology rings](../../../../../cohomology-ring.md) of the [product of two spheres](../../../../../product-of-two-spheres.md) and the [Complex projective plane](../../../../../complex-projective-plane.md).

For a map from the [Complex projective plane](../../../../../complex-projective-plane.md), write $f^*a=rx$ and $f^*b=sx$. Naturality of the [cup product](../../../../../cup-product.md) gives $r^2x^2=f^*(a^2)=0$ and $s^2x^2=f^*(b^2)=0$. Since $x^2$ has infinite order, $r=s=0$. It follows that $f^*(ab)=0$, so **every such map has degree $0$**.

In the reverse direction, write $g^*x=ra+sb$. Then

$$
g^*(x^2)=(ra+sb)^2=2rs\,ab,\qquad\boxed{\deg g=2rs\in2\mathbb Z.}
$$

Every even [mapping degree](../../../../../degree-of-a-continuous-mapping.md) really occurs. To construct it, identify $S^2$ with $\mathbb{CP}^1$ and use the [Segre embedding](../../../../../segre-embedding.md)

$$
\sigma:\mathbb{CP}^1\times\mathbb{CP}^1\longrightarrow\mathbb{CP}^3,\qquad
([z_0:z_1],[w_0:w_1])\longmapsto[z_0w_0:z_0w_1:z_1w_0:z_1w_1].
$$

The generator $x_3\in H^2(\mathbb{CP}^3;\mathbb Z)$ pulls back to $a+b$: restricting to either factor gives a projective line and hence coefficient $1$. By the [cellular approximation theorem](../../../../../cellular-approximation-theorem.md), $\sigma$ is homotopic to a [cellular map](../../../../../cellular-map.md). Its four-dimensional domain then maps into the four-skeleton $\mathbb{CP}^2$ of $\mathbb{CP}^3$. Denote that map by $g_0$; restriction of $x_3$ to $\mathbb{CP}^2$ is $x$, so $g_0^*x=a+b$ and $\deg g_0=2$.

For any integer $m$, choose a map $d_m:S^2\to S^2$ of [mapping degree](../../../../../degree-of-a-continuous-mapping.md) $m$. For $m>0$ one may use $z\mapsto z^m$ on the Riemann sphere, for $m<0$ use $z\mapsto\overline z^{\,|m|}$, and for $m=0$ use a constant map. Then $g_m=g_0\circ(d_m\times\operatorname{id})$ satisfies $g_m^*x=ma+b$, so **the possible degrees are exactly all even integers**, with $g_m$ realizing $2m$. The [cellular approximation](../../../../../cellular-approximation-theorem.md) here deforms this particular map into the skeleton; it does not require a retraction of $\mathbb{CP}^3$ onto $\mathbb{CP}^2$.

Finally, take the [connected sum of oriented manifolds](../../../../../connected-sum-of-oriented-manifolds.md) with both summands carrying their standard complex orientations. Its degree-two [cohomology](../../../../../cohomology-split.md) has generators $u,v$ with

$$
u^2=v^2=w,\qquad uv=0,\qquad\langle w,[\mathbb{CP}^2\mathbin\#\mathbb{CP}^2]\rangle=1.
$$

This follows by choosing the generators supported away from the two balls used to form the [connected sum](../../../../../connected-sum-of-oriented-manifolds.md), so mixed [cup products](../../../../../cup-product.md) vanish while each square gives the common orientation class. Write

$$
h^*u=ra+sb,\qquad h^*v=ta+zb,\qquad P=\begin{pmatrix}r&t\\s&z\end{pmatrix}.
$$

If $\deg h=n$, the three [cup product](../../../../../cup-product.md) relations say

$$
P^{\mathsf T}\begin{pmatrix}0&1\\1&0\end{pmatrix}P=nI_2.
$$

Taking determinants gives $-(\det P)^2=n^2$, which forces $n=0$. Therefore **the only possible degree to the connected sum is $0$**, realized by a constant map. This is a [degree constraint from intersection forms](../../../../../degree-constraint-from-intersection-forms.md): the indefinite [intersection form](../../../../../intersection-form.md) of the sphere product cannot pull back a definite form with a nonzero degree multiplier.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
