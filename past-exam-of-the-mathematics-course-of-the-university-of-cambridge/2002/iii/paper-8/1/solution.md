<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $0<q<\infty$, [weak type with a normed domain](../../../../../weak-type-with-a-normed-domain.md) means that there is a constant $C$ independent of $f\in E$ and $a>0$ such that

$$
\boxed{\lambda\{x:|Tf(x)|>a\}\leq\left(\frac{C\|f\|_E}{a}\right)^q}.
$$

Here $L^0$ consists of measurable functions modulo equality [almost everywhere](../../../../../almost-everywhere.md). A [sublinear operator](../../../../../sublinear-operator.md) satisfies absolute homogeneity and the pointwise domination $|T(f+g)|\leq|Tf|+|Tg|$. In particular the definition controls the output's superlevel measures, not necessarily its strong $L^q$ norm. At $q=\infty$, weak type is interpreted as the bound $\|Tf\|_\infty\leq C\|f\|_E$.

A useful theorem is [dense approximation under a weak-type maximal bound](../../../../../dense-approximation-under-a-weak-type-maximal-bound.md). Let $A_t:E\to L^0$ be [linear operators](../../../../../linear-operator.md) indexed by parameters tending to zero, and let $A_0:E\to L^0$ be another [linear operator](../../../../../linear-operator.md). Suppose there is a nonnegative [sublinear operator](../../../../../sublinear-operator.md) $S$ of weak type $(E,q)$ such that $|A_tf|,|A_0f|\leq Sf$, simultaneously in $t$ outside a null set for each input. Assume the suprema and limiting suprema used below are measurable. If $A_tg\to A_0g$ [almost everywhere](../../../../../almost-everywhere.md) for every $g$ in a dense subspace $D$, then $A_tf\to A_0f$ [almost everywhere](../../../../../almost-everywhere.md) for every $f\in E$. For a sequence of operators all suprema are automatically countable; continuously parametrized averages below also have measurable suprema.

To prove the theorem, fix $f$ and $g\in D$. Outside the exceptional sets for these inputs, [linearity](../../../../../linearity.md) and domination give

$$
\limsup_{t\to0}|A_tf-A_0f|\leq2S(f-g).
$$

Thus for every $a>0$ the set where this limiting error exceeds $a$ has measure at most $(2C\|f-g\|_E/a)^q$. Choose a sequence $g_k\in D$ converging to $f$ in norm and take the union of their null exceptional sets. Letting $k\to\infty$ makes the bound zero. Taking countably many positive rational $a$ proves convergence [almost everywhere](../../../../../almost-everywhere.md). This proves the requested sufficient condition rather than merely invoking a convergence theorem.

For the measure estimate, give finite [signed measures](../../../../../signed-measure.md) the [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md) $\|\nu\|=|\nu|(\mathbb R^d)$. The [uncentered maximal function of a finite measure](../../../../../uncentered-maximal-function-of-a-finite-measure.md) is sublinear because $|\nu+\eta|\leq|\nu|+|\eta|$. Its set $E_a=\{m_u\nu>a\}$ is open: it is precisely the union of open balls whose variation mass exceeds $a$ times their volume.

Fix a compact subset $K\subset E_a$ and select a finite cover of $K$ by these high-density balls. Order that finite collection by decreasing radius. Keep a ball if it is disjoint from all previously retained balls. Every discarded ball intersects a retained ball of at least its radius and is contained in that retained ball's triple dilation. The retained balls $B_j$ are disjoint and their triples cover $K$. Therefore

$$
\lambda(K)\leq\sum_j\lambda(3B_j)=3^d\sum_j\lambda(B_j)<\frac{3^d}{a}\sum_j|\nu|(B_j)\leq\frac{3^d\|\nu\|}{a}.
$$

By [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md), take the supremum over compact $K\subset E_a$ to obtain

$$
\boxed{\lambda\{m_u\nu>a\}\leq\frac{3^d}{a}\|\nu\|}.
$$

This is the [uncentered maximal weak-type inequality](../../../../../uncentered-maximal-weak-type-inequality.md), and proves weak type $(M(\mathbb R^d),1)$ even when the measure has atoms.

Finally work in dimension one. For $h\ne0$ define the [linear operator](../../../../../linear-operator.md)

$$
A_hf(x)=\frac{F(x+h)-F(x)}h=\frac1h\int_x^{x+h}f(t)\,dt.
$$

Its absolute value is bounded by $m_u(f\,dt)(x)$: first enlarge the interval slightly to put $x$ inside an open interval and then let the enlargement tend to zero. The endpoint masses vanish because $f\,dt$ is absolutely continuous. Taking $A_0f=f$, both operators are dominated by $Sf=m_u(f\,dt)+|f|$. The maximal bound and the [Markov inequality](../../../../../markov-inequality.md) give $\lambda\{Sf>a\}\leq2(3+1)\|f\|_1/a$.

Continuous compactly supported functions are dense in the [L1 space](../../../../../l1-space.md), and their averages tend to their values as $h\to0$ from either side. For a fixed $x$, the interval integral varies continuously for $h\ne0$, so the required suprema can be taken over rational $h$ and are measurable. Apply the proved weak-type theorem to conclude $A_hf(x)\to f(x)$ [almost everywhere](../../../../../almost-everywhere.md). Hence

$$
\boxed{F'(x)=f(x)\quad\text{for almost every }x}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
