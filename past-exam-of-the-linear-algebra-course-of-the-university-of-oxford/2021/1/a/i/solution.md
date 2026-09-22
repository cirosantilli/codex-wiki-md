<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

The [quotient vector space](../../../../../quotient-vector-space.md) $V/U$ identifies two [vectors](../../../../../vector.md) $v,w$ precisely when $v-w\in U$. Since $U$ is an [invariant subspace](../../../../../invariant-subspace.md), $T(U)\subseteq U$. Thus

$$
v+U=w+U\ \Longrightarrow\ v-w\in U\ \Longrightarrow\ T(v)-T(w)=T(v-w)\in U.
$$

Consequently $T(v)+U=T(w)+U$: the output does not depend on the chosen representative. This proves that the [induced linear map on a quotient vector space](../../../../../induced-linear-map-on-a-quotient-vector-space.md)

$$
\boxed{\overline T(v+U)=T(v)+U}
$$

is well-defined. It is a [linear map](../../../../../linear-map.md) because, for [scalars](../../../../../scalar.md) $a,b$,

$$
\overline T\bigl(a(v+U)+b(w+U)\bigr)
=T(av+bw)+U=a\overline T(v+U)+b\overline T(w+U).
$$

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
