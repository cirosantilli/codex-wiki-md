# Exponentially conjugated wave equation

↑ **Parent:** [Wave equation](wave-equation-split.md)

For real constants $\gamma,c$, the substitution $v=e^{\gamma t}u$ turns the displayed equation into the [wave equation](wave-equation-split.md) $v_{tt}=c^2v_{xx}$. If $u(x,0)=f(x)$ and $u_t(x,0)=g(x)$, then $v(x,0)=f(x)$ and $v_t(x,0)=g(x)+\gamma f(x)$. For $v_0=|c|>0$, [D'Alembert's formula](d-alembert-s-formula.md) consequently gives

$$
\boxed{u(x,t)=e^{-\gamma t}\left[\frac{f(x-v_0t)+f(x+v_0t)}2+\frac1{2v_0}\int_{x-v_0t}^{x+v_0t}[g(s)+\gamma f(s)]\,ds\right].}
$$

The extra $\gamma f$ term is necessary even when the original initial velocity is zero. For $c=0$, take the limit to obtain $u=e^{-\gamma t}[f+t(g+\gamma f)]$. The formula gives classical solutions for suitably smooth data and [weak solutions](weak-solution.md) for less regular data. Positive $\gamma$ damps the transformed wave, whereas negative $\gamma$ amplifies it.

## ↑ Ancestors (6)

1. [Wave equation](wave-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/5/ii/solution.md)
