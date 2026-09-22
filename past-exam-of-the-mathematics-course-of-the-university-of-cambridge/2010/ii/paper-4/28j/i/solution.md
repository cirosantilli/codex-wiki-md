<h1 id="28j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The requested properties are not properties of the optimum under the printed assumption $\alpha+\beta>1$.** We first derive their origin, and then solve the actual constrained problem.

Put $s=1-\ell$, so $0\le s\le1$, and write the [Hamiltonian of an optimal-control problem](../../../../../../hamiltonian-of-an-optimal-control-problem.md)

$$
H=c^\alpha s^\beta+p(rx+1-s-c).
$$

For an interior stationary control, $H_c=H_s=0$ gives

$$
p=\alpha c^{\alpha-1}s^\beta=\beta c^\alpha s^{\beta-1},
\qquad \beta c=\alpha s.
$$

This proves the printed identity only as a necessary stationarity condition for an interior candidate.

It fails the required maximization condition. For fixed positive $p$ and fixed $s$, maximization over $c$ gives

$$
c=\left(\frac{\alpha s^\beta}{p}\right)^{1/(1-\alpha)},\qquad
\max_c(H-prx)
=p(1-s)+(1-\alpha)
\left(\frac\alpha p\right)^{\alpha/(1-\alpha)}
s^{\beta/(1-\alpha)}.
$$

Since $\beta/(1-\alpha)>1$, this is strictly convex in $s$. Its maximum on $[0,1]$ is at an endpoint, not at its interior stationary point. Thus the actual optimum uses $\ell=1,c=0$, or $\ell=0,c>0$. On any consumption interval the printed relation would require $\beta c=\alpha$, although the actual optimal consumption varies with time.

This proves a genuine failure of the printed premise, not just failure to check a boundary condition. If the parameter inequality were reversed and an interior solution stayed within the control bounds, these first-order equations would instead arise from a concave objective.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
