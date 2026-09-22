<h1 id="minty-s-lemma">Minty's lemma</h1>

↑ **Parent:** [Monotone operator](monotone-operator.md)

For a [monotone operator](monotone-operator.md) $A:K\to X^*$ on a nonempty [convex set](convex-set-split.md) $K$ in a real [Banach space](banach-space-split.md), assume [hemicontinuity](hemicontinuity.md). Then $u\in K$ solves $\langle Au,v-u\rangle\geq0$ for every $v\in K$ if and only if $\langle Av,v-u\rangle\geq0$ for every $v\in K$. The quantifier applies to the entire inequality on each side.

The forward implication is [operator monotonicity](operator-monotonicity.md). For the reverse implication, choose $v=u+t(w-u)$ with $w\in K$ and $t>0$. Divide the assumed inequality by $t$ and pass to $t\downarrow0$ using [hemicontinuity](hemicontinuity.md); the result is $\langle Au,w-u\rangle\geq0$. For $K=X$, applying this to $A-f$ shows that $Au=f$ is equivalent to $\langle Av-f,v-u\rangle\geq0$ for every $v\in X$.

## ↑ Ancestors (6)

1. [Monotone operator](monotone-operator.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hemicontinuity](hemicontinuity.md)
- [Solution](past-exam-of-the-fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford/2023/3/a/solution.md)
