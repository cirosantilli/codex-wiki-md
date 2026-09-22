<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The defining rule for a [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md) is linear in the operator, so $\operatorname{Der}(\mathfrak g)$ is a [vector subspace](../../../../../vector-subspace.md) of the [general linear Lie algebra](../../../../../general-linear-lie-algebra.md) $\mathfrak{gl}(\mathfrak g)$. Its [Lie bracket](../../../../../lie-bracket.md) is the operator [commutator](../../../../../commutator.md). If $D,E$ are [derivations of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md), expand both compositions:

$$
\begin{aligned}
DE[x,y]&=[DEx,y]+[Ex,Dy]+[Dx,Ey]+[x,DEy],\\
ED[x,y]&=[EDx,y]+[Dx,Ey]+[Ex,Dy]+[x,EDy].
\end{aligned}
$$

Subtracting cancels the mixed terms and gives

$$
[D,E][x,y]=[[D,E]x,y]+[x,[D,E]y].
$$

Thus $[D,E]$ is again a [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md), proving that the [derivation Lie algebra](../../../../../derivation-lie-algebra.md) is a [Lie subalgebra](../../../../../lie-subalgebra.md) of $\mathfrak{gl}(\mathfrak g)$. This calculation works in every [characteristic of a field](../../../../../characteristic-of-a-field.md).

The [Jacobi identity](../../../../../jacobi-identity.md) states $[x,[y,z]]=[[x,y],z]+[y,[x,z]]$. It first shows that $\operatorname{ad}_x$ is a [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md), and then gives

$$
[\operatorname{ad}_x,\operatorname{ad}_y](z)=[x,[y,z]]-[y,[x,z]]=[[x,y],z].
$$

The map $x\mapsto\operatorname{ad}_x$ is linear, so this identity proves it is a [Lie algebra homomorphism](../../../../../lie-algebra-homomorphism.md).

Finally, for any [derivation of a Lie algebra](../../../../../derivation-of-a-lie-algebra.md) $D$,

$$
[D,\operatorname{ad}_x](y)=D[x,y]-[x,Dy]=[Dx,y].
$$

Consequently

$$
\boxed{[D,\operatorname{ad}_x]=\operatorname{ad}_{Dx},\qquad[\operatorname{Der}(\mathfrak g),\operatorname{ad}\mathfrak g]\subseteq\operatorname{ad}\mathfrak g.}
$$

This proves that the [inner derivations of a Lie algebra](../../../../../inner-derivation-of-a-lie-algebra.md) form an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) in $\operatorname{Der}(\mathfrak g)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
