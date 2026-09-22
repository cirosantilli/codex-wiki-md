<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [vectors](../../../../../../vector.md) in three-dimensional [Euclidean space](../../../../../../euclidean-norm.md), with the usual [dot product](../../../../../../dot-product.md) and [cross product](../../../../../../cross-product.md). The following explicit assignments compute the [circumcenter of a tetrahedron](../../../../../../circumcenter-of-a-tetrahedron.md):

$$
\begin{aligned}
u&\leftarrow B-A,&v&\leftarrow C-A,&w&\leftarrow D-A,\\
c_u&\leftarrow v\times w,&c_v&\leftarrow w\times u,&c_w&\leftarrow u\times v,\\
d&\leftarrow u\cdot c_u,&a&\leftarrow u\cdot u,&b&\leftarrow v\cdot v,&c&\leftarrow w\cdot w,\\
x&\leftarrow\frac{a c_u+b c_v+c c_w}{2d},&O&\leftarrow A+x.
\end{aligned}
$$

General position means $d\ne0$. The reciprocal cross-product identities give $x\cdot u=|u|^2/2$, $x\cdot v=|v|^2/2$ and $x\cdot w=|w|^2/2$. Consequently

$$
|O-B|^2-|O-A|^2=|x-u|^2-|x|^2=|u|^2-2x\cdot u=0,
$$

and likewise for $C,D$. Thus **$O$ is the unique point equidistant from the four vertices**. It can lie outside the [tetrahedron](../../../../../../tetrahedron.md); no inside constraint should be imposed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
