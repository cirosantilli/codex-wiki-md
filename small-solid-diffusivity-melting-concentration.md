# Small-solid-diffusivity melting concentration

↑ **Parent:** [Binary alloy Stefan similarity solution](binary-alloy-stefan-similarity-solution.md)

For $r=-\lambda>0$ and vanishing solid-to-liquid diffusivity ratio, $H(r)=\sqrt\pi r e^{r^2}\operatorname{erfc}(-r)$ gives the interfacial liquid [concentration](concentration.md). It increases from zero to $C_s$ as $r$ increases. Its [derivative](derivative.md) is $C_sH'/(1+H)^2$, which decreases from $\sqrt\pi C_s$ to zero. For a direct proof, write $A=H/r=\sqrt\pi e^{r^2}\operatorname{erfc}(-r)$. Then $A'=2rA+2$, so $A\geq\sqrt\pi+2r$. Differentiation gives $2H'^2-(1+H)H''=2[(1+r^2+2r^4)A^2+r(4r^2-1)A+2r^2-2]>0$: the bracket increases with $A$, and substitution of its lower bound gives only positive [polynomial](polynomial-split.md) coefficients, including constant $\pi-2$. Thus the [concentration](concentration.md) is strictly concave as a function of melting speed parameter $r$. Combining this with a linearized thermal balance produces one fold on the melting branch and, with the freezing branch, an interval of three possible interface speeds.

## ↑ Ancestors (7)

1. [Binary alloy Stefan similarity solution](binary-alloy-stefan-similarity-solution.md)
2. [Stefan problem](stefan-problem.md)
3. [Planetary ice shell](planetary-ice-shell.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-77/2/solution.md)
