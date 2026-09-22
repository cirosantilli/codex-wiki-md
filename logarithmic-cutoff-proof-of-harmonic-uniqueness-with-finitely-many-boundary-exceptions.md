# Logarithmic cutoff proof of harmonic uniqueness with finitely many boundary exceptions

↑ **Parent:** [Zero-boundary harmonic uniqueness](zero-boundary-harmonic-uniqueness.md)

Let $w$ be a bounded [harmonic function](harmonic-function.md) in a bounded connected smooth planar region, with zero continuous boundary limits except at finitely many points. Then $w=0$. This extends [zero-boundary harmonic uniqueness](zero-boundary-harmonic-uniqueness.md) to bounded solutions with isolated boundary exceptions, without assuming their initial [Dirichlet energy](dirichlet-energy.md) is finite.

Choose $\eta_\epsilon=0$ within distance $\epsilon^2$ of each exceptional point, $\eta_\epsilon=1$ beyond distance $\epsilon$, and interpolate linearly in the logarithm of distance. Each annular transition has $\int|\nabla\eta_\epsilon|^2=O(1/|\log\epsilon|)$. Apply the [divergence theorem](divergence-theorem.md) to the equation multiplied by $\eta_\epsilon^2w$. The ordinary boundary terms vanish, and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives

$$
\int\eta_\epsilon^2|\nabla w|^2\leq4\|w\|_\infty^2\int|\nabla\eta_\epsilon|^2\longrightarrow0.
$$

Every fixed compact subset eventually has $\eta_\epsilon=1$, so the [gradient](gradient.md) vanishes everywhere. The nonexceptional boundary data then fix the constant to zero. Differences of bounded [harmonic extensions](harmonic-extension.md) with identical piecewise continuous data satisfy this hypothesis. The individual extensions can have infinite [Dirichlet energy](dirichlet-energy.md) at a jump; the cutoff argument avoids applying an unjustified finite-energy identity to them.

## ↑ Ancestors (6)

1. [Zero-boundary harmonic uniqueness](zero-boundary-harmonic-uniqueness.md)
2. [Dirichlet problem](dirichlet-problem.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Exterior harmonic extension of disk boundary data](exterior-harmonic-extension-of-disk-boundary-data.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/2/solution.md)
