<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A finite extension is Galois when it is both normal and separable; over $\mathbb Q$ separability is automatic, so it is equivalently a [splitting field](../../../../splitting-field.md) of a [polynomial](../../../../polynomial-split.md) with distinct roots. Its [Galois group](../../../../galois-group.md) consists of the [field](../../../../field.md) [automorphisms](../../../../automorphism.md) fixing $\mathbb Q$. If $G=\operatorname{Gal}(L/\mathbb Q)$, the [Fundamental theorem of Galois theory](../../../../fundamental-theorem-of-galois-theory.md) gives mutually inverse inclusion-reversing bijections

$$
H\longmapsto L^H,\qquad K\longmapsto\operatorname{Gal}(L/K).
$$

They satisfy $[L:L^H]=|H|$ and $[L^H:\mathbb Q]=[G:H]$. The intermediate extension $K/\mathbb Q$ is Galois exactly when $H=\operatorname{Gal}(L/K)$ is normal, and then $\boxed{\operatorname{Gal}(K/\mathbb Q)\cong G/H}$ via restriction.

Every [permutation](../../../../permutation.md) of the four roots permutes the three unordered partitions into two pairs and hence permutes the three $\beta_j$. Thus each coefficient of $g(X)=\prod_{j=1}^3(X-\beta_j)$ is a [symmetric polynomial](../../../../symmetric-polynomial.md) in the four roots. The [Fundamental theorem of symmetric polynomials](../../../../fundamental-theorem-of-symmetric-polynomials.md) expresses it in the [elementary symmetric functions](../../../../elementary-symmetric-polynomial.md), which are rational coefficients of $f$. Hence $g\in\mathbb Q[X]$. Each product $\alpha_i\alpha_j$, $i<j$, occurs exactly twice in $\beta_1+\beta_2+\beta_3$, so that sum is $2q$. Therefore the quadratic coefficient is $\boxed{-2q}$.

For the given cubic write $g(X)=(X-2)^3+12$. The translated cubic $Y^3+12$ is Eisenstein at three, hence irreducible. It has one real root and a nonreal conjugate pair. Its [Galois group](../../../../galois-group.md) is transitive on three roots, so its order is divisible by three; [complex conjugation](../../../../complex-conjugation.md) is a [transposition](../../../../transposition-permutation.md). A [subgroup](../../../../subgroup.md) of $S_3$ with both a three-cycle and a [transposition](../../../../transposition-permutation.md) is all of $S_3$. Hence

$$
\boxed{\operatorname{Gal}(K/\mathbb Q)\cong S_3,\qquad[K:\mathbb Q]=6.}
$$

Let $G=\operatorname{Gal}(L/\mathbb Q)\le S_4$. Irreducibility of the quartic makes the root action transitive, so four divides $|G|$. The cubic [splitting field](../../../../splitting-field.md) $K$ lies inside $L$ by the definitions of the $\beta_j$, and restriction onto its [Galois group](../../../../galois-group.md) gives a quotient of order six. Thus six also divides $|G|$. Since $|G|$ divides 24, it is 12 or 24. If it were 12, the supplied index-two result would give $G=A_4$. The restriction kernel would then be a [normal subgroup](../../../../normal-subgroup.md) of $A_4$ of index six, contrary to the other supplied result. Thus

$$
\boxed{G=S_4.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
