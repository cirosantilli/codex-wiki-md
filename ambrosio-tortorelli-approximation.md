<h1 id="ambrosio-tortorelli-approximation">Ambrosio–Tortorelli approximation</h1>

↑ **Parent:** [Mumford–Shah functional](mumford-shah-functional.md)

The [Mumford–Shah functional](mumford-shah-functional.md) can be approximated by an auxiliary edge field $0\le v\le1$ and energy

$$
E_\varepsilon=\int(u-g)^2+\alpha(v^2+\eta_\varepsilon)|\nabla u|^2+\beta\left[\varepsilon|\nabla v|^2+\frac{(1-v)^2}{4\varepsilon}\right],\qquad0<\eta_\varepsilon=o(\varepsilon).
$$

The field is near one inside regions and near zero across an [image edge](image-edge.md), weakening smoothing there. The profile $v(s)=1-e^{-|s|/(2\varepsilon)}$ has unit edge energy per unit length in this normalization. The [1990 construction](https://onlinelibrary.wiley.com/doi/10.1002/cpa.3160430805) is a [Gamma-convergence](gamma-convergence.md) approximation; its global-minimizer [limit](limit-of-a-function.md) does not guarantee global optimality of an alternating numerical solve. Each fixed-field subproblem is quadratic, but the joint energy is nonconvex.

## ↑ Ancestors (5)

1. [Mumford–Shah functional](mumford-shah-functional.md)
2. [Variational image processing](variational-image-processing.md)
3. [Image processing](image-processing.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gamma-convergence](gamma-convergence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64/4/solution.md)
