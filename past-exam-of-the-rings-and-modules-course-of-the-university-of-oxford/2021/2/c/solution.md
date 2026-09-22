<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $K=\ker\phi$, $H=\ker\psi$, and $Q=\operatorname{Im}q$. The [kernel of a module homomorphism](../../../../kernel-of-a-module-homomorphism.md) $H$ is a [submodule](../../../../submodule.md), so its image $L=q(H)$ is a [submodule](../../../../submodule.md). For $x\in H$, $\phi(q(x))=\psi(x)=0$, showing $L\subseteq K$. Thus the [quotient module](../../../../quotient-module.md) $K/L$ exists. Also $L\subseteq Q$.

Consider the restriction to $K$ of the natural [module homomorphism](../../../../module-homomorphism.md) $R^m\to R^m/Q$:

$$
\alpha:K\longrightarrow R^m/Q,\qquad y\longmapsto y+Q.
$$

Its [kernel of a module homomorphism](../../../../kernel-of-a-module-homomorphism.md) is $K\cap Q$. We have $L\subseteq K\cap Q$. Conversely, if $y\in K\cap Q$, choose $x\in R^n$ with $y=q(x)$. Then

$$
\psi(x)=\phi(q(x))=\phi(y)=0,
$$

so $x\in H$ and $y\in L$. Hence $\boxed{K\cap Q=L}$.

The map $\alpha$ is [surjective](../../../../surjective-function.md). Given $v+Q\in R^m/Q$, use the [surjectivity](../../../../surjective-function.md) of $\psi$ to choose $x\in R^n$ with $\psi(x)=\phi(v)$. Set $y=v-q(x)$. Then

$$
\phi(y)=\phi(v)-\psi(x)=0,\qquad y+Q=v+Q.
$$

Thus $y\in K$ is a preimage of the arbitrary class $v+Q$.

By the [first isomorphism theorem for modules](../../../../first-isomorphism-theorem-for-modules.md), $\alpha$ induces the [module isomorphism](../../../../module-isomorphism.md)

$$
\boxed{\overline\alpha:\ker\phi/L\xrightarrow{\ \cong\ }R^m/\operatorname{Im}q,\qquad
y+L\longmapsto y+\operatorname{Im}q}.
$$

Explicitly, replacing $y$ by $y+\ell$ with $\ell\in L$ leaves its class modulo $Q$ unchanged, proving well-definedness. Its formula preserves [addition](../../../../addition.md) and [scalar multiplication](../../../../scalar-multiplication.md). If its value is zero, $y\in K\cap Q=L$, so $y+L=0$, proving [injectivity](../../../../injective-function.md); [surjectivity](../../../../surjective-function.md) was proved above. These checks give all the requested properties of the induced map.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
