# Cubic FitzHugh-Nagumo nullcline criterion

↑ **Parent:** [FitzHugh-Nagumo model](fitzhugh-nagumo-model.md)

For $\dot v=v(\alpha-v)(v-1)-w+I$, $\dot w=\beta v-\gamma w$, set $k=\beta/\gamma$. Intersections of the [nullclines](nullcline.md) solve $I=h(v)=v^3-(1+\alpha)v^2+(\alpha+k)v$. Three simple [equilibria](equilibrium-point-of-a-dynamical-system.md) are possible precisely when $k<M=(1-\alpha+\alpha^2)/3$ and $h(u_+)<I<h(u_-)$, where $u_\pm=(1+\alpha\pm\sqrt{1-\alpha+\alpha^2-3k})/3$. To prove this, observe that $h'=k-M+3(v-(1+\alpha)/3)^2$ has two real zeros exactly when $k<M$; monotonicity on the three resulting intervals counts the intersections. At either endpoint there are a double and a simple root, and at $k=M$, $I=h((1+\alpha)/3)$ there is one triple root.

## ↑ Ancestors (5)

1. [FitzHugh-Nagumo model](fitzhugh-nagumo-model.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-further-mathematical-biology-course-of-the-university-of-oxford/2023/2/a/i/solution.md)
