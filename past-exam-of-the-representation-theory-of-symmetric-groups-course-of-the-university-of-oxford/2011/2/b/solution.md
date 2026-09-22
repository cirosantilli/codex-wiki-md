<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $W=S_F^{(n-2,1,1)}$ and let $H\cong S_{n-1}$ be the [subgroup](../../../../subgroup.md) fixing one. For $\tau=(r,s)\in H$, let $u=\min\{\tau(i),\tau(j)\}$ and $v=\max\{\tau(i),\tau(j)\}$. Permuting a tableau's entries and then ordering its first column gives

$$
\boxed{\tau e_{1ij}=\begin{cases}e_{1uv},&\tau(i)<\tau(j),\\-e_{1uv},&\tau(i)>\tau(j).\end{cases}}
$$

The underlying [basis](../../../../basis.md) element is $e_{1ij}$ exactly when $\tau$ preserves the unordered pair $\{i,j\}$: either $\{r,s\}=\{i,j\}$, giving the minus sign, or the two pairs are disjoint, giving the plus sign.

If $p\neq2$, invariance of $x$ under $(i,j)$ forces its $e_{1ij}$ [coefficient](../../../../coefficient.md) to satisfy $a_{ij}=-a_{ij}$, because no other [basis vector](../../../../basis-vector.md) is sent to that [basis vector](../../../../basis-vector.md). Thus every [coefficient](../../../../coefficient.md) vanishes. Consequently $W^H=0$, and in particular $W^{S_n}=0$, so there is no nonzero [homomorphism](../../../../homomorphism.md) from the trivial [module](../../../../module-mathematics.md). Any [homomorphism](../../../../homomorphism.md) $M_F^{(n-1,1)}\to W$ is determined by the [image](../../../../image-of-a-function.md) of its [tabloid](../../../../tabloid.md) with singleton row $\{1\}$. That [image](../../../../image-of-a-function.md) is fixed by $H$ and is zero, making the whole [homomorphism](../../../../homomorphism.md) zero.

**The printed vanishing assertion is false in [characteristic two](../../../../characteristic-two.md).** Signs then coincide, so $H$ permutes the [basis](../../../../basis.md) indexed by unordered pairs from $\{2,\ldots,n\}$. This action is [transitive](../../../../transitive-relation.md), and

$$
\boxed{W^H=Fv,\qquad v=\sum_{2\leq i<j\leq n}e_{1ij}\neq0\quad(p=2).}
$$

The vector is nonzero by standard-basis independence. It also gives a nonzero map from the [permutation module](../../../../permutation-module.md): send the singleton-row [basis vector](../../../../basis-vector.md) indexed by $r$ to $g_rv$, where $g_r(1)=r$. This is well defined because two choices of $g_r$ differ by an element of $H$, and it is $S_n$-equivariant by construction. Thus the claimed vanishing of permutation-module [homomorphisms](../../../../homomorphism.md) fails for every $n\geq4$ in [characteristic two](../../../../characteristic-two.md).

The full-group fixed space can be determined explicitly. Denote a [hook](../../../../hook-of-a-young-diagram.md) [tabloid](../../../../tabloid.md) by $[a,b]$, recording its second- and third-row entries. In [characteristic two](../../../../characteristic-two.md), $e_{1ij}$ is the sum of the six [tabloids](../../../../tabloid.md) using ordered pairs from $\{1,i,j\}$. In $v$, a [tabloid](../../../../tabloid.md) whose two recorded entries both differ from one appears once; a [tabloid](../../../../tabloid.md) using one appears $n-2$ times. Hence for odd $n$, $v$ is the sum of all [hook](../../../../hook-of-a-young-diagram.md) [tabloids](../../../../tabloid.md) and is fixed by $S_n$. For even $n$, it is the sum of precisely the [tabloids](../../../../tabloid.md) avoiding one and is moved by $(1,2)$. Since every full-group fixed vector already lies in $Fv$, the corrected [dimensions](../../../../dimension-vector-space.md) are

$$
\boxed{\begin{array}{c|cc}
&\dim W^H&\dim W^{S_n}\\\hline
p\neq2&0&0\\
p=2,\ n\text{ even}&1&0\\
p=2,\ n\text{ odd}&1&1
\end{array}}
$$

Thus even the trivial-module vanishing fails for odd $n$ in [characteristic two](../../../../characteristic-two.md); for example $n=5$ gives the explicit nonzero [invariant](../../../../invariant-mathematics.md) $v$. These corrected fixed spaces allow the valid later conclusions to be proved in all characteristics.

The corrected parity dependence is described by [fixed vectors in a hook Specht module in characteristic two](../../../../fixed-vectors-in-a-hook-specht-module-in-characteristic-two.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the representation Theory of Symmetric Groups course of the University of Oxford](../../../split.md)
5. [Representation Theory of Symmetric Groups course of the University of Oxford](../../../../representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
