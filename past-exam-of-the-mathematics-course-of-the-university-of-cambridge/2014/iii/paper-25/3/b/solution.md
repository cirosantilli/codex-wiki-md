<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here is a quantitative local form of the [Landau zero-free-region theorem](../../../../../../landau-zero-free-region-theorem.md). Let $t\ge2$, $0<\eta\le1/4$, $M\ge2$, and suppose $|\zeta(z)|\le M$ on the two closed discs of radius $\eta$ centred at $1+\eta/4+it$ and $1+\eta/4+2it$. Then every zero $\beta+it$ satisfies

$$
\boxed{1-\beta\ge\frac{c\eta}{1+\log(M/\eta)}}
$$

for an absolute positive $c$. In particular, if upper bounds of this form hold locally for every large height, they give a zero-free region of this width. The discs are away from the [pole](../../../../../../pole.md), and the [Euler product](../../../../../../euler-product.md) excludes zeros to the right of one.

We state precisely the permitted [local logarithmic-derivative lemma](../../../../../../local-logarithmic-derivative-lemma.md). If $f$ is holomorphic on a neighborhood of $|z-z_0|\le R$, $f(z_0)\ne0$, and $|f|\le M$, then for $|z-z_0|\le R/3$ away from zeros,

$$
\frac{f'(z)}{f(z)}=\sum_{|\rho-z_0|\le R/2}\frac1{z-\rho}+O\left(\frac{1+\log(M/|f(z_0)|)}R\right).
$$

The zeros are counted with multiplicity. This standard disc estimate, which may be assumed here, follows by factoring nearby zeros and applying a [Cauchy estimate for derivatives](../../../../../../cauchy-estimate.md) to the remaining logarithm. When every zero has real part at most one and $\Re z>1$, the zero terms have nonnegative real parts, giving the required lower bound. The estimate with fixed radius ratios is also recorded as Lemma 24.17 in [Montgomery and Vaughan's general treatment](https://personal.science.psu.edu/rcv4/Vol3/Vol3.pdf).

The reciprocal [Euler product](../../../../../../euler-product.md) gives $|\zeta(1+\eta/4+ij t)|\ge1/\zeta(1+\eta/4)\gg\eta$ for $j=1,2$. Put $B=1+\log(M/\eta)$. The lemma's error on both discs is therefore $O(B/\eta)$. Let $d=1-\beta$. If $d\ge\eta/24$, the desired conclusion already holds after reducing $c$. Otherwise $\beta+it$ is among the local zeros and, for $1<\sigma\le1+\eta/4$,

$$
\Re\frac{\zeta'(\sigma+it)}{\zeta(\sigma+it)}\ge\frac1{\sigma-\beta}-C\frac B\eta,\qquad\Re\frac{\zeta'(\sigma+2it)}{\zeta(\sigma+2it)}\ge-C\frac B\eta.
$$

All other zero terms may be discarded because their real parts are nonnegative. The simple [pole](../../../../../../pole.md) at one gives $-\zeta'(\sigma)/\zeta(\sigma)=(\sigma-1)^{-1}+O(1)$. Insert these inequalities into part (a):

$$
\frac4{\sigma-\beta}-\frac3{\sigma-1}\ll\frac B\eta.
$$

There is no zero on the line one by the argument in Question 2(a), so $d>0$. Choose $\sigma=1+6d$, which lies in the indicated range. The left side is $(4/7-3/6)/d=1/(14d)$. Hence $d\gg\eta/B$, proving the theorem. The logarithm of the upper bound, rather than the upper bound itself, is what enters the zero-free width.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
