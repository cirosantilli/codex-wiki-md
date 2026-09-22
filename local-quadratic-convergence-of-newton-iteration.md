# Local quadratic convergence of Newton iteration

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)

Let $F$ be twice [continuously differentiable](continuously-differentiable-function.md) on an interval around a [zero of a function](zero-of-a-function.md) $t_*$, with $|F'(t)|\geq m>0$ and $|F''(t)|\leq M$ there. Choose a closed interval $[t_*-\rho,t_*+\rho]$ inside that interval with $M\rho/(2m)<1$. Starting inside it makes the [Newton root-finding iteration](newton-root-finding-iteration.md) well defined, keeps it inside, and gives the displayed [quadratic convergence](quadratic-convergence.md) bound for $e_r=t_r-t_*$. The nonzero [derivative](derivative.md) and sufficiently close start are essential hypotheses. The scalar estimate follows from the [Taylor remainder](taylor-remainder.md) argument in MIT's root-finding notes.[Laurent Demanet, MIT 18.330, Chapter 4, pp. 2–3, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/5b325bfa56a599794c7196de926844b0_MIT18_330S12_Chapter4.pdf)

For a short proof outline, apply [Taylor's theorem](taylor-s-theorem.md) between $t_r$ and $t_*$; subtract the defining [tangent line](tangent-line.md) equation. The linear error cancels, leaving $e_{r+1}=F''(\xi_r)e_r^2/(2F'(t_r))$. The displayed bound shrinks the error and preserves the chosen interval. If $F''(t_*)\ne0$, the error ratio tends to $|F''(t_*)/(2F'(t_*))|$; if it vanishes, convergence can be faster.

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
