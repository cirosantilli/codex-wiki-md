<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use the sign convention $E(\phi)=\delta S_0/\delta\phi$ from part [b](../b.md), and let

$$
S_\eta[\phi]=S_0[\phi]+\eta\int d^4x\,f(\phi)E(\phi).
$$

In the [path integral](../../../../path-integral.md), make the local [field redefinition](../../../../field-redefinition.md) $\phi_{\rm old}=\chi-\eta f(\chi)$. The [functional Taylor expansion](../../../../functional-taylor-expansion.md) of the [action](../../../../action.md) gives

$$
\begin{aligned}
S_0[\chi-\eta f(\chi)]
&=S_0[\chi]-\eta\int d^4x\,f(\chi)\frac{\delta S_0}{\delta\chi(x)}+O(\eta^2),\\
\eta\int d^4x\,f(\phi_{\rm old})E(\phi_{\rm old})
&=\eta\int d^4x\,f(\chi)E(\chi)+O(\eta^2).
\end{aligned}
$$

The two first-order terms cancel. Neglecting the [functional Jacobian](../../../../functional-jacobian.md) as permitted,

$$
\boxed{Z_\eta=\mathcal N\int\mathcal D\chi\,\exp\{iS_0[\chi]+O(\eta^2)\}.}
$$

Thus $fE$ is a [redundant operator](../../../../redundant-operator.md) at first order, by the [equivalence theorem for field redefinitions](../../../../equivalence-theorem-for-field-redefinitions.md). The same argument works for a local derivative-dependent $f$, which is needed to remove $(\Box\phi)^2$. Insertions and sources must be transformed too: arbitrary untransformed [off shell](../../../../off-shell.md) [correlation functions](../../../../correlation-function.md) need not be equal.

**Sign qualification.** If instead $E_+=\Box\phi+m^2\phi+\lambda\phi^3/6$ is used, then $E_+=-\delta S_0/\delta\phi$. An added $+\eta fE_+$ is removed by $\phi_{\rm old}=\chi+\eta f(\chi)$. The minus shift requested in the source therefore fixes which sign is meant by its otherwise unspecified $E$.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
