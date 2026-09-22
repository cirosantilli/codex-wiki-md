<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $M>a\ge0$ and $N>b\ge0$, define

$$
\boxed{K_{a,b}^{M,N}=\langle x^M,y^N,t(a,b)\rangle\le K.}
$$

The [normal form theorem for a free product](../../../../../../normal-form-theorem-for-a-free-product.md) gives

$$
K_{a,b}^{M,N}\cong\langle X,Y,T\mid XY=YX\rangle\cong\mathbb Z^2*\mathbb Z,
$$

where $X,Y,T$ map to $x^M,y^N,t(a,b)$. To see injectivity, expand an alternating word in $\langle x^M,y^N\rangle$ and powers of $t(a,b)$. The conjugating $x,y$ factors commute with the lattice syllables, so each intervening nonidentity lattice syllable stays nonidentity in the expanded free-product normal form.

Its intersection with $T_K$ is the [free group](../../../../../../free-group.md) with basis

$$
K_{a,b}^{M,N}\cap T_K
=\langle t(Mu+a,Nv+b):u,v\in\mathbb Z\rangle.
$$

This follows by moving all $x^M,y^N$ factors to the right; the zero-exponent lattice remainder characterizes membership in the kernel.

The required [isomorphisms](../../../../../../isomorphism.md) are specified on the three generators by

$$
\boxed{\phi_i:x^m\mapsto x^{m^2},\quad y^m\mapsto y,\quad t(a_i,b_i)\mapsto t(c_i,0),}
$$

and

$$
\boxed{\varphi_j:x^m\mapsto x,\quad y^m\mapsto y^{m^2},\quad t(a_j,b_j)\mapsto t(0,c_j).}
$$

Each source and target has the same presentation $\langle X,Y,T\mid[X,Y]=1\rangle$, and each displayed assignment identifies its three abstract generators. Hence these are genuine [isomorphisms](../../../../../../isomorphism.md), not merely maps of generating sets.

On the kernel basis they give exactly the machine transitions:

$$
\phi_i\bigl(t(mu+a_i,mv+b_i)\bigr)=t(m^2u+c_i,v),
$$



$$
\varphi_j\bigl(t(mu+a_j,mv+b_j)\bigr)=t(u,m^2v+c_j).
$$

For example, rewrite the first input as $x^{-mu}y^{-mv}t(a_i,b_i)x^{mu}y^{mv}$ and apply $\phi_i$ to each factor. These identities also hold for negative $u,v$, since they are identities in the [groups](../../../../../../group-split.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
