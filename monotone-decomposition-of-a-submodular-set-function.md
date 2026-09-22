# Monotone decomposition of a submodular set function

↑ **Parent:** [Submodular set function](submodular-set-function.md)

Every real-valued [submodular set function](submodular-set-function.md) on a finite [ground set](ground-set.md) $V$ is the sum of a [normalised set function](normalised-set-function.md) $g$ that is nonnegative, monotone and submodular, and a [modular set function](modular-set-function.md) $h$. A useful explicit choice is

$$
d_x=f(V)-f(V\setminus\{x\}),\qquad
h(S)=f(\varnothing)+\sum_{x\in S}d_x,\qquad g=f-h.
$$

**Proof.** The formula makes $h$ a [modular set function](modular-set-function.md), so $g$ is a [submodular set function](submodular-set-function.md). It is a [normalised set function](normalised-set-function.md) because $h(\varnothing)=f(\varnothing)$. For $x\notin S$, [diminishing returns](diminishing-returns-characterization-of-submodularity.md) gives $\Delta_x f(S)\geq\Delta_x f(V\setminus\{x\})=d_x$, hence $\Delta_xg(S)\geq0$. Thus $g$ is a [monotone set function](monotone-set-function.md), and starting at zero makes it a [nonnegative function](nonnegative-function.md). The decomposition separates all potentially negative terminal [marginal increments](marginal-increment-of-a-set-function.md) into the simple additive term. A constant term in $h$ is necessary unless $f$ is already a [normalised set function](normalised-set-function.md).

## ↑ Ancestors (8)

1. [Submodular set function](submodular-set-function.md)
2. [Set function](set-function.md)
3. [Function](function-split.md)
4. [Set theory](set-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/1/f/solution.md)
