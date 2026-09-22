# Global Picard iteration with a decaying kernel

↑ **Parent:** [Picard iteration](picard-iteration.md)

Consider the [Volterra integral equation](volterra-integral-equation.md)

$$
y(t)=b h(t)+\int_0^tK(t,s)y(s)^2\,ds,\qquad t\geq0,
$$

where $h$ is continuous, $|h|\leq1$, $h(0)=1$, and the continuous kernel satisfies $0\leq K(t,s)\leq e^{-c(t-s)}$ for $0\leq s\leq t$, with $c>0$. If $0<|b|<c/4$, there is exactly one continuous solution on the whole half-line. It is bounded, and [Picard iteration](picard-iteration.md) beginning at $y_0=bh$ converges in [supremum norm](supremum-norm.md) with contraction ratio at most $\gamma=4|b|/c<1$.

For a proof, the integral of the kernel is at most $1/c$. Thus $T$ maps the closed ball of radius $2|b|$ in the [Banach space](banach-space-split.md) of [bounded continuous functions](bounded-continuous-functions.md) into itself, since $\|Ty\|_\infty\leq|b|+4b^2/c<2|b|$. Factoring $y^2-v^2$ gives $\|Ty-Tv\|_\infty\leq\gamma\|y-v\|_\infty$ on this ball. The [contraction mapping theorem](contraction-mapping-theorem.md) gives its unique fixed point. A [first-exit argument](first-exit-argument.md) shows that every continuous solution, even one not initially assumed bounded, stays strictly inside the same ball: a first time with $|y|=2|b|$ would contradict $|y|\leq|b|+4b^2/c$. Reapplying the estimate gives the strict global bound $\|y\|_\infty\leq|b|(1+\gamma)<2|b|$, so uniqueness is unrestricted within the continuous solution class. If $b=0$, zero is the only solution by the [Gronwall inequality](gronwall-inequality.md) on each finite interval.

## ↑ Ancestors (8)

1. [Picard iteration](picard-iteration.md)
2. [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2023/1/b/iii/solution.md)
- [Picard iterate](picard-iterate.md)
