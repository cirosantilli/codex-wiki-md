<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the bilinear pairing $T_g(f)=\int_{\mathbb R^n}fg$, so the map $g\mapsto T_g$ is complex linear. With the sesquilinear convention $\int f\overline g$ the representing map would instead be conjugate linear. For [conjugate exponents](../../../../../../conjugate-exponents.md) $p,q$, [Hölder's inequality](../../../../../../holder-s-inequality.md) gives $|T_g(f)|\leq\|g\|_q\|f\|_p$. If $g\ne0$, take $v=|g|^{q-2}\overline g$, defined as zero where $g=0$. Then

$$
\int vg=\|g\|_q^q,\qquad \|v\|_p=\|g\|_q^{q/p},\qquad q-q/p=1.
$$

Consequently **$\|T_g\|=\|g\|_q$**. This also proves [injectivity](../../../../../../injective-function.md) of the representation.

For [surjectivity](../../../../../../surjective-function.md), let $\ell$ be a nonzero element of the [continuous dual space](../../../../../../continuous-dual-space-split.md) of $L^p$ and choose $f_0$ with $\ell(f_0)=1$. Its kernel $K$ is a [closed linear subspace](../../../../../../closed-vector-subspace.md). Use the allowed best-approximation fact to choose $h\in K$ and put $z=f_0-h$. Thus $\ell(z)=1$ and

$$
\Phi(k):=\int |z|^{p-2}\overline z\,k=0\quad(k\in K),\qquad \Phi(z)=\|z\|_p^p>0.
$$

For each $f$, the vector $f-\ell(f)z$ belongs to $K$. Therefore $\Phi(f)=\ell(f)\|z\|_p^p$, giving

$$
\boxed{\ell(f)=\int fg,\qquad g=\frac{|z|^{p-2}\overline z}{\|z\|_p^p}\in L^q,\qquad \|\ell\|=\|g\|_q.}
$$

Membership follows from $(p-1)q=p$; the zero functional is represented by zero. This proves the isometric isomorphism $(L^p(\mathbb R^n))^*\cong L^q(\mathbb R^n)$ without using a representation theorem as a substitute for the proof. It is the [closed-hyperplane proof of Lp duality](../../../../../../closed-hyperplane-proof-of-lp-duality.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
