# Empty and open feasible regions

↑ **Parent:** [Feasible region](feasible-region.md)

Adding an [optimization constraint](optimization-constraint.md) removes possibilities: if it permits a [set](set-split.md) $C$, the new [feasible region](feasible-region.md) is $F\cap C\subseteq F$. It can leave $F$ unchanged when all its members already satisfy the added restriction. For a fixed [objective function](objective-function.md), restricting the [feasible set](feasible-region.md) cannot lower a [minimization problem](minimization-problem.md)'s [infimum](infimum.md). In the [equality slice of a feasible triangle](equality-slice-of-a-feasible-triangle.md), it raises the attained value from $0.5$ to $1$.

Instead add $x+y\geq4$ to the [feasible triangle with a squared-distance objective](feasible-triangle-with-a-squared-distance-objective.md). No point can have both $x+y\leq3$ and $x+y\geq4$. The resulting [feasible set](feasible-region.md) is the [empty set](empty-set.md), so there is no [feasible point](feasible-point.md) and no optimizing decision. Under the extended-value convention for a [minimization problem](minimization-problem.md), its [infimum](infimum.md) is $+\infty$.[§4.1.1, printed p. 127: infeasibility and the empty-set infimum convention](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

A nonempty [feasible set](feasible-region.md) can also lack an optimizing decision. With domain $D=\mathbb R$, minimize $f(x)=x$ subject to the strict [inequality](inequality-mathematics.md) $x>0$. The [feasible region](feasible-region.md) $(0,\infty)$ is an [open set](open-set.md). Its [infimum](infimum.md) is $0$, approached by the [feasible points](feasible-point.md) $x_n=1/n$, but $0$ is excluded. Every [feasible point](feasible-point.md) $x$ is beaten by $x/2$, so no [minimum](minimum-of-a-subset-of-a-total-order.md) is attained. Replacing $x>0$ by $x\geq0$ includes the missing optimum. Open [feasible regions](feasible-region.md) do not always prevent attainment: minimizing $(x-1)^2$ on the same [open set](open-set.md) attains value $0$ at $x=1$. A useful sufficient condition is instead the [extreme value theorem](extreme-value-theorem.md): a [continuous](continuous-function.md) [objective function](objective-function.md) on a nonempty [compact set](compact-space.md) attains its [minimum](minimum-of-a-subset-of-a-total-order.md).

## ↑ Ancestors (6)

1. [Feasible region](feasible-region.md)
2. [Feasible point](feasible-point.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
