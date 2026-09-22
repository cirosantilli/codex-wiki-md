<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $I=[N]$ and let $f=1_A-\delta1_I$ be the balanced [indicator function](../../../../../indicator-function.md), extended by zero to the [integers](../../../../../integer.md). For finitely supported functions define the [linear configuration count](../../../../../linear-configuration-count.md)

$$
\Lambda(g_1,g_2,g_3)=\sum_{x+z=2y}g_1(x)g_2(y)g_3(z).
$$

Since $A$ has no nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md), $\Lambda(1_A,1_A,1_A)=|A|=\delta N$. On the other hand, $\Lambda(1_I,1_I,1_I)\geq N^2/4$. Hence, once $N$ is sufficiently large in terms of $\delta$,

$$
\left|\Lambda(1_A,1_A,1_A)-\delta^3\Lambda(1_I,1_I,1_I)\right|\geq c_0\delta^3N^2
$$

for an absolute $c_0>0$.

Use the unnormalized [Fourier transform](../../../../../fourier-transform.md) $\widehat h(\theta)=\sum_xh(x)e(-\theta x)$ on $\mathbb R/\mathbb Z$. Telescoping $1_A=\delta1_I+f$ writes the preceding difference as

$$
\Lambda(f,1_A,1_A)+\delta\Lambda(1_I,f,1_A)+\delta^2\Lambda(1_I,1_I,f).
$$

Let $M=\|\widehat f\|_\infty$. The Fourier-integral formula for $\Lambda$, followed by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the [Parseval identity](../../../../../parseval-identity.md), bounds these three terms respectively by

$$
M\delta N,qquad M\delta^{3/2}N,qquad M\delta^2N.
$$

They are all at most $M\delta N$, so

$$
M\geq c_1\delta^2N
$$

for an absolute $c_1>0$. Choose $\theta$ with $|\widehat f(\theta)|=M$.

By the [Dirichlet approximation theorem](../../../../../dirichlet-s-approximation-theorem.md), some integer $1\leq d\leq\sqrt N$ satisfies $\|d\theta\|_{\mathbb R/\mathbb Z}\leq N^{-1/2}$. Choose a sufficiently small absolute multiple $\eta$ of $\delta^2$. Partition each residue-class progression of common difference $d$ into progressions $P_j$ whose lengths lie between $\eta\sqrt N$ and $2\eta\sqrt N$; for sufficiently large $N$, short final pieces can be joined to the preceding piece. On each $P_j$, the [linear phase](../../../../../linear-phase.md) $e(-\theta x)$ varies by at most $4\pi\eta$. Choosing $\eta$ small enough compared with $c_1\delta^2$ therefore yields

$$
\sum_j\left|\sum_{x\in P_j}f(x)\right|
\geq |\widehat f(\theta)|-4\pi\eta N
\geq\frac{c_1}{2}\delta^2N.
$$

The sums over all cells add to $\sum_If=0$, so their positive parts total half their absolute values. At least one $P_j$ consequently satisfies

$$
\sum_{x\in P_j}f(x)\geq\frac{c_1}{4}\delta^2|P_j|.
$$

This is the [Roth density-increment step](../../../../../roth-density-increment-step.md), and it gives

$$
\boxed{|P_j|\geq\eta\sqrt N,qquad |A\cap P_j|\geq(\delta+c\delta^2)|P_j|}
$$

with $c=c_1/4$ and $\eta>0$ depending only on $\delta$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 147](../../paper-147-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
