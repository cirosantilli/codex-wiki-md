<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the connectivity hypothesis in its usual based sense: $X$ is $(n-2)$-connected, with $n\ge2$ for the nontrivial suspension range. Form the suspension as two cones $C_-X$ and $C_+X$ meeting in $X$. Both cones are [contractible](../../../../../contractible-space.md). Their relative [homotopy](../../../../../homotopy.md) sequences give $\pi_j(C_\pm X,X)\cong\pi_{j-1}(X)$ in the relevant degrees, so both cone pairs are $(n-1)$-connected.

The [homotopy excision theorem](../../../../../homotopy-excision-theorem.md) says that if two [CW pairs](../../../../../cw-pair.md) meeting in a connected subcomplex are $p$- and $q$-connected, $p,q\ge1$, the map from the first relative pair to the union relative to the second part is an [isomorphism](../../../../../isomorphism.md) in degrees $i<p+q$ and a surjection in degree $p+q$. Here $p=q=n-1$, giving

$$
\pi_i(C_+X,X)\longrightarrow\pi_i(\Sigma X,C_-X)
$$

as an [isomorphism](../../../../../isomorphism.md) for $i<2n-2$ and a surjection for $i=2n-2$. Contractibility identifies the domain with $\pi_{i-1}(X)$ and the target with $\pi_i(\Sigma X)$. The comparison under these identifications is the suspension map: a [sphere](../../../../../sphere.md) representative is coned in each half and the two cones give its suspended [sphere](../../../../../sphere.md) representative. Hence the [Freudenthal suspension from two cones](../../../../../freudenthal-suspension-from-two-cones.md) proves

$$
\boxed{\pi_{i-1}(X)\to\pi_i(\Sigma X)\text{ is onto for }i\le2n-2,\text{ and is an isomorphism for }i<2n-2.}
$$

For connected [CW complexes](../../../../../cw-complex.md), reduced and unreduced suspension have the same based [homotopy](../../../../../homotopy.md) type, so either standard suspension convention gives this result. In the low-dimensional range, [pointed sets](../../../../../pointed-set.md) are used where necessary; the displayed positive-degree [homomorphism](../../../../../homomorphism.md) assertion concerns the usual [groups](../../../../../group-split.md).

For $S^r$ with $r\ge2$, cellular approximation makes every [sphere](../../../../../sphere.md) map of degree below $r$ [null-homotopic](../../../../../null-homotopic-map.md): it can be homotoped into the point skeleton of the CW structure having cells only in degrees zero and $r$. The [Hurewicz theorem](../../../../../hurewicz-theorem.md) therefore identifies its first possible nonzero [homotopy group](../../../../../homotopy-group.md) with [homology](../../../../../homology-split.md). Its [cellular chain complex](../../../../../cellular-chain-complex.md) gives $H_r(S^r;\mathbb Z)=\mathbb Z$. For $r=1$, lifting a based loop to the [universal cover](../../../../../universal-cover.md) $\mathbb R\to S^1$ classifies it by an integer endpoint displacement, so $\pi_1(S^1)=\mathbb Z$; the degree-one Hurewicz map is [abelianization](../../../../../abelianization.md) and is an [isomorphism](../../../../../isomorphism.md) here. Thus

$$
\boxed{\pi_r(S^r)\cong H_r(S^r;\mathbb Z)\cong\mathbb Z\qquad(r\ge1).}
$$

Alternatively, after the $r=2$ Hurewicz base case, the suspension [isomorphisms](../../../../../isomorphism.md) above propagate the generator to every higher [sphere](../../../../../sphere.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
