<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [continuous embedding](../../../../continuous-embedding.md) $X\hookrightarrow Y$ is an injective continuous linear inclusion, so $\|x\|_Y\leq C\|x\|_X$ for a fixed constant. On a finite-measure domain, [Holder inequality](../../../../holder-inequality.md) gives

$$
\boxed{\|u\|_q\leq|\Omega|^{1/q-1/p}\|u\|_p\quad(1\leq q\leq p\leq\infty),}
$$

with $1/\infty=0$. For finite $p>q$ apply [Holder inequality](../../../../holder-inequality.md) to $|u|^q\cdot1$ with exponents $p/q$ and $p/(p-q)$; equality of exponents is immediate, and $p=\infty$ follows by integrating the supremum bound.

[Weak convergence](../../../../weak-convergence.md) $u_j\rightharpoonup u$ means $\ell(u_j)\to\ell(u)$ for every [bounded linear functional](../../../../continuous-linear-functional.md) $\ell\in X^*$. The [Riemann-Lebesgue lemma](../../../../riemann-lebesgue-lemma.md) says that the [Fourier transform](../../../../fourier-transform-split.md) of an integrable function tends to zero at high frequency. Since $L^2(0,1)\subset L^1(0,1)$, it makes $\cos(j\pi x)$ weakly null in $L^2$. Its absolute value is at most one, so $u_jv_j\in L^2$. For a test $\phi\in L^2$,

$$
\left|\int u_j(v_j-v)\phi\right|\leq\|v_j-v\|_2\|\phi\|_2\to0,
$$

while $\int u_jv\phi\to0$ by the [Riemann-Lebesgue lemma](../../../../riemann-lebesgue-lemma.md) applied to $v\phi\in L^1$. Hence **$u_jv_j\rightharpoonup0$**. Taking $w_j=u_j=\cos(j\pi x)$ instead gives $u_jw_j=(1+\cos(2j\pi x))/2\rightharpoonup1/2$, so two weakly null factors need not have a weakly null product.

For $\bar z_j=j^{1/p}\mathbf1_{(0,1/j)}$ and $p'=p/(p-1)$, [Holder inequality](../../../../holder-inequality.md) gives

$$
\left|\int\bar z_jg\right|\leq\left(\int_0^{1/j}|g|^{p'}\right)^{1/p'}\to0\quad(g\in L^{p'}).
$$

Thus **$\bar z_j\rightharpoonup0$ in $L^p$**. In contrast, if $z_j$ had a weak $L^1$ limit $z$, testing on every interval strictly away from zero would give integral zero for $z$, hence $z=0$ [almost everywhere](../../../../almost-everywhere.md) by the permitted fact. Testing against the constant function one would give $\int z=1$, a contradiction. Therefore **$z_j$ has no weak $L^1$ limit**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
