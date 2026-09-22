<h1 id="a/a1/solution">Solution</h1>

↑ **Parent:** [A1](../a1.md)

A [group action](../../../../group-action-split.md) is a map $G\times\Omega\to\Omega$, $(g,\omega)\mapsto g\omega$, satisfying $1\omega=\omega$ and $(gh)\omega=g(h\omega)$. Its [group orbit](../../../../orbit-group-theory.md) and [stabilizer](../../../../stabilizer-subgroup.md) are

$$
\boxed{\operatorname{Orb}(\omega)=\{g\omega:g\in G\},\qquad
G_\omega=\{g\in G:g\omega=\omega\}.}
$$

The [stabilizer](../../../../stabilizer-subgroup.md) contains the identity. If $g,h$ fix $\omega$, then $gh$ fixes it; and $g\omega=\omega$ implies $g^{-1}\omega=\omega$ after applying $g^{-1}$. Thus it is a [subgroup](../../../../subgroup.md).

The map from left [cosets](../../../../coset.md) $gG_\omega$ to group-orbit points $g\omega$ is well-defined, surjective and injective: $g\omega=h\omega$ is equivalent to $h^{-1}g\in G_\omega$. Therefore $|\operatorname{Orb}(\omega)|=[G:G_\omega]=|G|/|G_\omega|$ for finite $G$.

For [conjugation](../../../../conjugation.md) in $S_3$, the [group orbits](../../../../orbit-group-theory.md) are exactly the conjugacy classes, determined by [cycle type](../../../../cycle-type.md):

$$
\boxed{\{1\},\qquad\{(12),(13),(23)\},\qquad\{(123),(132)\}.}
$$

[Conjugation](../../../../conjugation.md) sends $(i_1\cdots i_k)$ to $(g(i_1)\cdots g(i_k))$, so these displayed sets are invariant and each is one [group orbit](../../../../orbit-group-theory.md). Their sizes $1,3,2$ also agree with [centralizer](../../../../centralizer.md) orders $6,2,3$.

## ↑ Ancestors (12)

1. [A1](../a1.md)
2. [A](../../a.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
