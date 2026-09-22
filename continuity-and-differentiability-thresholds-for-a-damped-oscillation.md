# Continuity and differentiability thresholds for a damped oscillation

↑ **Parent:** [Differentiable function](differentiable-function.md)

Suppose $h$ is bounded by one in [absolute value](absolute-value.md) on a punctured neighbourhood of zero. Suppose also that there are positive [sequences](sequence.md) $p_n,q_n\to0$ with $h(p_n)=1$ and $h(q_n)=0$. Extend $F_a(x)=|x|^ah(x)$ by $F_a(0)=0$. Then

$$
F_a\text{ is continuous at zero}\iff a>0,
\qquad
F_a\text{ is differentiable at zero}\iff a>1.
$$

When the [derivative](derivative.md) exists, it equals zero. For [continuity](continuous-function.md), the bound $|F_a(x)|\leq|x|^a$ gives the [epsilon-delta definition of continuity](epsilon-delta-definition-of-continuity.md) with $\delta=\varepsilon^{1/a}$ when $a>0$. If $a\leq0$, the values $F_a(p_n)=p_n^a$ remain at least one for sufficiently large $n$, contradicting [continuity](continuous-function.md) at zero.

For [differentiability](differentiability.md), the [difference quotient](difference-quotient.md) is bounded in [absolute value](absolute-value.md) by $|x|^{a-1}$, so it tends to zero when $a>1$. Conversely its values along $q_n$ are zero, forcing any possible [derivative](derivative.md) to be zero. Its values along $p_n$ equal $p_n^{a-1}$ and fail to tend to zero when $a\leq1$.

For example, $h(x)=\sin(\pi\sin(1/x))$ has the required positive [sequences](sequence.md) $p_n=1/(2\pi n+\pi/6)$ and $q_n=1/(2\pi n)$. This separates the suppression needed for [continuity](continuous-function.md) from the stronger suppression needed for [differentiability](differentiability.md).

## ↑ Ancestors (5)

1. [Differentiable function](differentiable-function.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-1/20/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/19/b/ii/solution.md)
