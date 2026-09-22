<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [principal bundle](../../../../../principal-bundle.md) with structural Lie group $G$ is locally a product $U\times G$, with changes of trivialization of the form $(x,g)\mapsto(x,t(x)g)$. Define a right action locally by $(x,g)\cdot h=(x,gh)$. It is independent of trivialization because $t(x)(gh)=(t(x)g)h$. It is smooth and obeys the group-action law. Right multiplication in $G$ is free and transitive, so the global action is free and each fiber is a single orbit. Equivalently these properties and equivariant local triviality can be included in the definition of a principal bundle.

For a representation $\rho:G\to GL(V)$, form the [associated vector bundle](../../../../../associated-vector-bundle.md)

$$
\boxed{E=P\times_\rho V=(P\times V)/\bigl[(p,v)\sim(ph,\rho(h)^{-1}v)\bigr].}
$$

Projection sends $[p,v]$ to the base point of $p$. A local section $s(x)$ gives coordinates $[s(x),v]$ and hence a local product $U\times V$; on overlaps the principal transition functions act through $\rho$. Because these maps are linear in $v$, the fibers have well-defined vector-space structures.

For an $n$-dimensional manifold, its [frame bundle](../../../../../frame-bundle.md) has points $u:\mathbb R^n\to T_xM$ that are linear isomorphisms. Right action is composition $u\cdot A=u\circ A$ for $A\in GL(n,\mathbb R)$. Coordinate frames provide local trivializations. Its associated bundle for the defining representation is the [tangent bundle](../../../../../tangent-bundle.md), by the well-defined map $[u,v]\mapsto u(v)$. A metric restricts the frames to linear isometries and reduces the group to $O(r,s)$; choosing orientation gives the corresponding special-orthogonal reduction.

In Minkowski spacetime choose a reference oriented pseudo-orthonormal frame at the origin. Every such frame is specified by its base point $a\in\mathbb R^{3,1}$ and a Lorentz transformation $L\in SO(3,1)$. The [Poincaré group](../../../../../poincare-group.md) has multiplication

$$
(a,L)(b,M)=(a+Lb,LM),
$$

and its right Lorentz action is $(a,L)\cdot h=(a,Lh)$. Hence

$$
\boxed{E(3,1)=\mathbb R^{3,1}\rtimes SO(3,1)\ \longrightarrow\
E(3,1)/SO(3,1)\cong\mathbb R^{3,1},\qquad\pi(a,L)=a}
$$

is the [oriented orthonormal frame bundle of Minkowski spacetime](../../../../../oriented-orthonormal-frame-bundle-of-minkowski-spacetime.md). The same argument with $O(3,1)$ gives the full unoriented bundle. If time orientation is fixed, use the orthochronous components throughout; the use of $SO$ in the printed quotient is an orientation reduction.

For four-dimensional [de Sitter spacetime](../../../../../de-sitter-spacetime.md), use the spacelike hyperboloid $x\cdot x=\ell^2$ in $\mathbb R^{4,1}$. An element of $SO(4,1)$ maps a fixed unit spacelike vector to $x/\ell$, and its other columns give an oriented pseudo-orthonormal tangent frame. The stabilizer of that unit vector is $SO(3,1)$. This identifies the [oriented frame bundle of de Sitter spacetime](../../../../../oriented-frame-bundle-of-de-sitter-spacetime.md) and its projection:

$$
\boxed{SO(4,1)\longrightarrow\mathrm{dS}_4=SO(4,1)/SO(3,1).}
$$

The right stabilizer action changes the tangent frame without changing $x$.

For [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md), take $x\cdot x=-\ell^2$ in $\mathbb R^{3,2}$. A unit timelike normal has orthogonal complement of signature $(3,1)$, so its stabilizer is again $SO(3,1)$. Appending this normal to a tangent frame realizes the [oriented orthonormal frame bundle of anti-de Sitter spacetime](../../../../../oriented-orthonormal-frame-bundle-of-anti-de-sitter-spacetime.md) as

$$
\boxed{SO(3,2)\longrightarrow\mathrm{AdS}_4=SO(3,2)/SO(3,1).}
$$

Connected components or orientation/time-orientation restrictions must be chosen consistently. This quotient is the anti-de Sitter quadric, which has a periodic timelike coordinate. If “anti-de Sitter spacetime” denotes its universal cover, pull the frame bundle back to that cover, rather than identify the covered spacetime with the unmodified quotient.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
