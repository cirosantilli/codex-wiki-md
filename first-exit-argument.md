# First-exit argument

↑ **Parent:** [Differential inequality](differential-inequality.md)

A first-exit argument proves preservation of a bound by contradiction at the earliest time the bound could fail. Continuity of the evolving quantity ensures that, if a trajectory starts inside a closed region and later leaves it, there is a first contact with its boundary. An estimate valid up to that contact can then rule the contact out. This is useful before a global [supremum norm](supremum-norm.md) is known to be finite.

For example, suppose a continuous $y$ with $|y(0)|<R$ satisfies $|y(t)|\leq B+c\max_{0\leq s\leq t}|y(s)|^2$, where $B+cR^2<R$. At a first time $T$ with $|y(T)|=R$, the estimate gives $R\leq B+cR^2<R$, a contradiction. Hence $|y(t)|<R$ for every finite time. A separate uniform estimate is needed to conclude $\sup_{t\geq0}|y(t)|<R$, since pointwise strict inequalities alone allow equality of the supremum.

## ↑ Ancestors (7)

1. [Differential inequality](differential-inequality.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Global Picard iteration with a decaying kernel](global-picard-iteration-with-a-decaying-kernel.md)
- [Solution](past-exam-of-the-differential-equations-1-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
