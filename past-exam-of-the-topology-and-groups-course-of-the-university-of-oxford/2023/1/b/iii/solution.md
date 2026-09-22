<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Identify the bottom $j(X)=q(X\times\{0\})$ with $X$; its natural map $j$ is a [topological embedding](../../../../../topological-embedding.md). To verify this directly, an [open subset](../../../../../open-set.md) $O\subseteq X$ gives the saturated [open subset](../../../../../open-set.md) $O\times[0,1/2)$ of the space before taking the [quotient topology](../../../../../quotient-topology.md); its image is open in $M(f)$ and meets the bottom in $j(O)$.

Suppose first that there is a [retraction](../../../../../retraction.md) $R:M(f)\to j(X)$. Define the [continuous map](../../../../../continuous-map.md)

$$
g=j^{-1}Ri:Y\longrightarrow X.
$$

Then

$$
L(x,t)=j^{-1}R(q(x,t))
$$

is a [homotopy](../../../../../homotopy-split.md) with $L(x,0)=x$ and $L(x,1)=g(f(x))$. Hence $gf\simeq\operatorname{id}_X$.

Conversely, suppose a [continuous map](../../../../../continuous-map.md) $g:Y\to X$ has $gf\simeq\operatorname{id}_X$. Reverse the parameter if necessary to choose a [homotopy](../../../../../homotopy-split.md) $L$ with $L(x,0)=x$ and $L(x,1)=gf(x)$. Set

$$
R(q(x,t))=j(L(x,t)),\qquad R(i(y))=j(g(y)).
$$

At the glued end, $j(L(x,1))=j(gf(x))$, exactly the value prescribed at $i(f(x))$. The [universal property of the quotient topology](../../../../../universal-property-of-the-quotient-topology.md) therefore gives a [continuous map](../../../../../continuous-map.md) $R:M(f)\to j(X)$. At the bottom, $R(j(x))=j(x)$, proving that $R$ is a [retraction](../../../../../retraction.md). We have established the [mapping-cylinder bottom retraction criterion](../../../../../mapping-cylinder-bottom-retraction-criterion.md):

$$
\boxed{j(X)\text{ is a retract of }M(f)\iff\exists g:Y\to X\text{ continuous with }gf\simeq\operatorname{id}_X.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
