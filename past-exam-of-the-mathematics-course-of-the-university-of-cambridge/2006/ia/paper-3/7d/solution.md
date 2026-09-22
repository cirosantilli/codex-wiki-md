<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Since $\sigma$ is a [group homomorphism](../../../../../group-homomorphism.md), $\sigma(0)=I$, $\sigma(x+y)=\sigma(x)\sigma(y)$, and $\sigma(-x)=\sigma(x)^{-1}$. The product is closed on $\mathbb R\times\mathbb R^2$. Its two associative bracketings give

$$
\begin{aligned}
[(x,v)*(y,w)]*(z,u)
&=(x+y+z,v+\sigma(x)w+\sigma(x+y)u),\\
(x,v)*[(y,w)*(z,u)]
&=(x+y+z,v+\sigma(x)w+\sigma(x)\sigma(y)u),
\end{aligned}
$$

and coincide by the homomorphism property. The [identity element](../../../../../identity-element.md) is $(0,0)$, and the two-sided inverse is

$$
\boxed{(x,v)^{-1}=(-x,-\sigma(-x)v)}.
$$

For example, multiplying on the right gives $v-\sigma(x)\sigma(-x)v=0$, and multiplying on the left gives $-\sigma(-x)v+\sigma(-x)v=0$. Thus this law defines a [group](../../../../../group-split.md), specifically a [semidirect product](../../../../../semidirect-product.md).

If it is an [abelian group](../../../../../abelian-group.md), comparing $(x,0)*(0,w)$ and $(0,w)*(x,0)$ gives $\sigma(x)w=w$ for every $w$. Hence $\sigma(x)=I$ for every $x$. Conversely this trivial action makes the product ordinary vector addition. Therefore **the unique action giving a commutative group is**

$$
\boxed{\sigma(x)=I\quad\text{for all }x}.
$$

For the final condition, compare $(0,ae_1)*(x,w)$ and $(x,w)*(0,ae_1)$. They are $(x,ae_1+w)$ and $(x,w+\sigma(x)ae_1)$ respectively. They coincide for every $a,x,w$ exactly when $\sigma(x)e_1=e_1$ for every $x$. The first column of $\sigma(x)$ is then $(1,0)^{\mathsf T}$; since it lies in the [special linear group](../../../../../special-linear-group.md), its determinant is one and its other diagonal entry is also one. Thus

$$
\sigma(x)=\begin{pmatrix}1&r(x)\\0&1\end{pmatrix}.
$$

Matrix multiplication gives $r(x+y)=r(x)+r(y)$. Conversely any such [additive function](../../../../../additive-function.md) gives a homomorphism into $SL(2,\mathbb R)$ fixing $e_1$ and therefore makes these translations central. This proves the full characterization of the [central translations in a linear semidirect product](../../../../../central-translations-in-a-linear-semidirect-product.md):

$$
\boxed{r:(\mathbb R,+)\longrightarrow(\mathbb R,+)\text{ may be any homomorphism}}.
$$

No continuity or measurability is assumed, so it would be unjustified to restrict the answer to $r(x)=cx$.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
