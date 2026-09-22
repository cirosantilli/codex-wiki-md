<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $z=x-y$ and $d\Pi_p=d^3\mathbf p/[(2\pi)^3 2E_{\mathbf p}]$. The [Dirac adjoint](../../../../dirac-adjoint.md) of the printed [mode expansion of a Dirac field](../../../../mode-expansion-of-a-dirac-field.md) is

$$
\bar\psi_a(x)=\int\frac{d^3\mathbf p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}\sum_s
\left[e^{ip\cdot x}a^{s\dagger}_{\mathbf p}\bar u_a^s(\mathbf p)+e^{-ip\cdot x}b^s_{\mathbf p}\bar v_a^s(\mathbf p)\right].
$$

The [Fock vacuum](../../../../fock-vacuum.md) is annihilated by $a,b$. The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) therefore give the two non-time-ordered [vacuum expectation values](../../../../vacuum-expectation-value.md)

$$
\begin{aligned}
\langle0|\bar\psi_a(x)\psi_b(y)|0\rangle&=\int d\Pi_p\,e^{-ip\cdot z}\sum_s\bar v_a^s(\mathbf p)v_b^s(\mathbf p),\\
\langle0|\psi_b(y)\bar\psi_a(x)|0\rangle&=\int d\Pi_p\,e^{ip\cdot z}\sum_s\bar u_a^s(\mathbf p)u_b^s(\mathbf p).
\end{aligned}
$$

In the first line, the only surviving contraction is $\langle b b^\dagger\rangle$; in the second it is $\langle a a^\dagger\rangle$. Both of these unordered contractions have positive coefficients.

However, [fermionic time ordering](../../../../fermionic-time-ordering.md) includes a minus sign when it interchanges two odd fields:

$$
T\bar\psi_a(x)\psi_b(y)=\theta(z^0)\bar\psi_a(x)\psi_b(y)-\theta(-z^0)\psi_b(y)\bar\psi_a(x).
$$

Thus the result following from the stated [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) and standard [time ordering](../../../../time-ordering.md) is

$$
\boxed{\begin{aligned}
C_{ab}(x,y)&\equiv\langle0|T\bar\psi_a(x)\psi_b(y)|0\rangle\\
&=\int d\Pi_p\left[\theta(z^0)e^{-ip\cdot z}\sum_s\bar v_a^s v_b^s
-\theta(-z^0)e^{ip\cdot z}\sum_s\bar u_a^s u_b^s\right].
\end{aligned}}
$$

**The second term printed with a plus sign is not correct for standard [fermionic time ordering](../../../../fermionic-time-ordering.md).** Its plus-plus expression would be an ungraded chronological product. The missing minus cannot be absorbed by a phase choice for $u$ or $v$, since each [spin sum](../../../../spin-sum.md) contains a spinor and its adjoint.

For comparison with the conventional [Dirac propagator](../../../../dirac-propagator.md), define $S_F(w)_{ba}=\langle0|T\psi_b(w)\bar\psi_a(0)|0\rangle$ and let $\mu$ denote this free [Dirac field](../../../../dirac-field.md)'s mass. Then

$$
\boxed{C_{ab}(x,y)=-S_F(y-x)_{ba}
=-\int\frac{d^4p}{(2\pi)^4}\frac{i(\not{p}+\mu)_{ba}}{p^2-\mu^2+i0}\,e^{-ip\cdot(y-x)}.}
$$

The exchange of the spinor indices is essential: $\bar v_a v_b$ is the $(b,a)$ component of $v\bar v$, not its $(a,b)$ component.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
