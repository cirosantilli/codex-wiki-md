# Time and distance averages of speed

↑ **Parent:** [Speed](speed.md)

For forward motion with nonnegative [speed](speed.md) $v(t)$ over duration $T>0$ and distance $L=\int_0^Tv(t)\,dt>0$, define the time-averaged [speed](speed.md) $V_t=L/T$ and distance-averaged [speed](speed.md) $V_x=L^{-1}\int v\,dx$. The [change of variables](change-of-variables-formula.md) $dx=v\,dt$ gives $V_x=\mathbb E_t[v^2]/\mathbb E_t[v]$, where $\mathbb E_t$ averages uniformly over time. Therefore

$$
V_x-V_t=\frac{\mathbb E_t[v^2]-(\mathbb E_t[v])^2}{\mathbb E_t[v]}=\frac{\operatorname{Var}_t(v)}{V_t}\geq0.
$$

Equality holds exactly for constant [speed](speed.md) almost everywhere. This also follows directly from the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) applied to $v$ and one on the time interval. The reason for the difference is that distance averaging puts more weight on periods when the vehicle covers more distance per unit time. These formulas assume a finite second time moment; if that moment is infinite, the distance average is infinite and the inequality holds in the extended sense.

## ↑ Ancestors (7)

1. [Speed](speed.md)
2. [Velocity](velocity.md)
3. [Position](position.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/20/b/solution.md)
