<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [complex tautological line bundle](../../../../../../complex-tautological-line-bundle.md) on $\mathbb P^1$ has fibre at a line $\ell\subseteq\mathbb C^2$ equal to $\ell$ itself:

$$
\mathcal O_{\mathbb P^1}(-1)=\{(\ell,v):v\in\ell\}\subseteq\mathbb P^1\times\mathbb C^2.
$$

Define $\mathcal O(1)=\mathcal O(-1)^*$, $\mathcal O(k)=\mathcal O(1)^{\otimes k}$ for $k>0$, $\mathcal O(0)$ to be trivial, and $\mathcal O(k)=\mathcal O(-1)^{\otimes(-k)}$ for $k<0$. These are the [tensor powers of the hyperplane line bundle](../../../../../../tensor-powers-of-the-hyperplane-line-bundle.md).

On the two given charts, use the [holomorphic local frames](../../../../../../holomorphic-local-trivialization.md) $e_0(w)=(1,w)$ and $e_1(z)=(z,1)$ of $\mathcal O(-1)$. The maps $([1:w],a)\mapsto([1:w],a(1,w))$ and $([z:1],b)\mapsto([z:1],b(z,1))$ are its trivializations. On the overlap $z=1/w$,

$$
e_1=z e_0=w^{-1}e_0,
\qquad a e_0=b e_1\iff b=wa.
$$

Thus the frame-transition factor from $e_0$ to $e_1$ is $w^{-1}$, while the fibre-coordinate transition from chart 0 to chart 1 is $w$. Specifying both avoids an inverse-convention ambiguity.

For $\mathcal O(k)$, let $e_i^{(k)}$ be the induced frames; they satisfy $e_1^{(k)}=w^k e_0^{(k)}$. Identifying overlap sections using $e_0^{(k)}$, the [Čech cochain groups](../../../../../../cech-cochain-group.md) and [Čech coboundary](../../../../../../cech-coboundary.md) for $k\geq0$ are

$$
\boxed{C^0=\mathcal O(\mathbb C)\oplus\mathcal O(\mathbb C),\qquad
C^1=\mathcal O(\mathbb C^*),\qquad
\delta(a,b)(w)=w^k b(1/w)-a(w).}
$$

Here $\mathcal O(\mathbb C)$ means entire functions in the coordinate of the corresponding chart. Global sections are $\ker\delta$, so $a(w)=w^k b(1/w)$, or $b(z)=z^k a(1/z)$. Expanding the entire function $a(w)=\sum_{j\geq0}a_jw^j$ shows that $b$ is holomorphic at zero exactly when $a_j=0$ for $j>k$. Thus a global section is determined by a polynomial of degree at most $k$, with basis $1,w,\ldots,w^k$ in the chart-0 frame. Therefore **$\boxed{\dim H^0(\mathbb P^1,\mathcal O(k))=k+1\quad(k\geq0)}$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
