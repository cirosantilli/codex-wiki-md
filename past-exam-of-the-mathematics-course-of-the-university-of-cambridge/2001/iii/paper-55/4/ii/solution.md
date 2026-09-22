<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the geometric properties of the [Feigenbaum geometric potential](../../../../../../feigenbaum-geometric-potential.md): for some constants $0<b\leq B<\infty$,

$$
-B\leq U\leq-b<0,\qquad \operatorname{var}_rU\leq C\vartheta^r,\quad0<\vartheta<1.
$$

Here $\operatorname{var}_r$ means variation between sequences agreeing in their first $r$ symbols. In particular $D=\sum_{r\geq1}\operatorname{var}_rU<\infty$. These are the standard bounds for the [Feigenbaum geometric potential](../../../../../../feigenbaum-geometric-potential.md); the [symbolic potential](../../../../../../symbolic-potential.md) is not the singular expression $-\log|g'|$ at a quadratic critical point.

First allow all $n$ spins and use a fixed remote tail $\eta$, writing $Z_n(\gamma;\eta)$ for the weighted [partition function](../../../../../../canonical-partition-function.md). In a concatenated block of lengths $n$ and $m$, replacing the history before the second block by $\eta$ changes its energy by at most $D$: the $j$th summand has the same first $j$ symbols, so its difference is at most $\operatorname{var}_jU$. Therefore

$$
e^{-|\gamma|D}Z_n(\gamma;\eta)Z_m(\gamma;\eta)
\leq Z_{n+m}(\gamma;\eta)
\leq e^{|\gamma|D}Z_n(\gamma;\eta)Z_m(\gamma;\eta).
$$

For $a_n=\log Z_n$, the [almost-additive partition-function limit](../../../../../../almost-additive-partition-function-limit.md) follows explicitly: $a_n+|\gamma|D$ is subadditive and $a_n-|\gamma|D$ superadditive, so [Fekete's lemma](../../../../../../fekete-s-lemma.md) gives the same finite limit for both after division by $n$. The finiteness follows from bounded $U$ and the $2^n$ words.

Changing the fixed remote tail also changes each full energy by at most $D$. The question fixes the first spin to one and sums the remaining $n-1$ spins; its [partition function](../../../../../../canonical-partition-function.md) is $e^{\gamma U(1,0,0,\ldots)}Z_{n-1}(\gamma;(1,0,0,\ldots))$. The tail comparison and bounded first contribution show that its normalized logarithm has the same limit. Thus the requested $f(\gamma)$ exists and equals the [topological pressure](../../../../../../topological-pressure.md) of $\gamma U$.

For any $\delta>0$, every length-$n$ energy lies between $-Bn$ and $-bn$, hence

$$
e^{-Bn\delta}Z_n(\gamma)\leq Z_n(\gamma+\delta)\leq e^{-bn\delta}Z_n(\gamma).
$$

Taking normalized logarithms and limits gives

$$
\boxed{-B\delta\leq f(\gamma+\delta)-f(\gamma)\leq-b\delta.}
$$

So $f$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) and strictly decreasing. For each finite $n$, differentiation of the log-sum gives $f_n''(\gamma)=n^{-1}\operatorname{Var}_{n,\gamma}(H_n)\geq0$. Thus $f_n$ is [convex](../../../../../../convex-function.md), and passing to its finite pointwise limit proves that $f$ is [convex](../../../../../../convex-function.md) too.

At zero weight the prescribed sum has $2^{n-1}$ terms, so $f(0)=\log2$. For $\gamma>0$ the preceding bounds give $\log2-B\gamma\leq f(\gamma)\leq\log2-b\gamma$. The function therefore becomes negative at sufficiently large positive $\gamma$. Continuity and strict decrease prove

$$
\boxed{\text{There is exactly one }\gamma_*>0\text{ with }f(\gamma_*)=0,\qquad
\frac{\log2}{B}\leq\gamma_*\leq\frac{\log2}{b}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
