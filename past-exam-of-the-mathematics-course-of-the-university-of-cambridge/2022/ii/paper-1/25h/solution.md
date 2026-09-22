<h1 id="25h/solution">Solution</h1>

↑ **Parent:** [25H](../25h.md)

For an irreducible [algebraic variety](../../../../../algebraic-variety.md) $X$ and $p\in X$, the local ring $\mathcal O_{X,p}$ consists of germs of [rational functions](../../../../../rational-function.md) regular on a neighbourhood of $p$. If $X\subseteq\mathbb A^n$ has ideal $I(X)$, its [Zariski tangent space](../../../../../zariski-tangent-space.md) is

$$
T_pX=\{v\in k^n:df_p(v)=0\text{ for every }f\in I(X)\}.
$$

The given variety is the [blowup of the affine plane at the origin](../../../../../blowup-of-the-affine-plane-at-the-origin.md). On the chart $W\ne0$, put $W=1$; then $Y=XZ$, so $(X,Z)$ are free affine coordinates. On the chart $Z\ne0$, put $Z=1$; then $X=WY$, so $(W,Y)$ are free affine coordinates. These two smooth affine-plane charts cover $V$, hence every point of $V$ is smooth.

If $(X,Y)\ne(0,0)$, the equation forces

$$
[W:Z]=[X:Y].
$$

Consequently $\pi$ restricts to an isomorphism away from the origin, and is therefore [birational](../../../../../birational-variety.md). Above the origin, however,

$$
\pi^{-1}(0,0)=\{(0,0)\}\times\mathbb P^1,
$$

so $\pi$ is not injective and cannot be an [isomorphism of algebraic varieties](../../../../../isomorphism-of-algebraic-varieties.md). Birationality gives

$$
\boxed{k(V)=k(\mathbb A^2)=k(X,Y)}.
$$

For any morphism $\varphi:V\to V'$ with $V'$ affine, its restriction to the exceptional curve $E\cong\mathbb P^1$ is constant: every regular function on a projective line is constant, and the affine coordinate functions of $V'$ therefore have constant pullbacks. Since $E$ has more than one point, $\varphi$ is not injective. If $V$ itself were affine, its identity morphism would contradict this conclusion, so $V$ is not affine.

Over $\mathbb C$, $V$ is not compact in the Euclidean topology: the sequence $(n,0,[1:0])$ has no convergent subsequence. Every complex [projective variety](../../../../../projective-variety.md) is Euclidean compact. Since [compactness](../../../../../compact-space.md) is preserved by homeomorphisms, $V$ cannot be homeomorphic to a projective variety.

## ↑ Ancestors (10)

1. [25H](../25h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
