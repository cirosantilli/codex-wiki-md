<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

For a reversible change of a simple compressible system with fixed composition, the first law is

$$
\boxed{dE=T\,dS-P\,dV.}
$$

An adiabatic change exchanges no heat. A reversible adiabatic change is isentropic, $dS=0$; adiabatic alone does not imply constant [entropy](../../../../../entropy.md) for an irreversible process.

Define the [Helmholtz free energy](../../../../../helmholtz-free-energy.md) $F=E-TS$. Then $dF=-S\,dT-P\,dV$. Equality of its mixed partial derivatives gives the [Maxwell relation](../../../../../maxwell-relations.md)

$$
\boxed{\left(\frac{\partial S}{\partial V}\right)_T
=\left(\frac{\partial P}{\partial T}\right)_V.}
$$

Holding $T$ fixed in the first law and using this relation gives

$$
\boxed{\left(\frac{\partial E}{\partial V}\right)_T
=T\left(\frac{\partial P}{\partial T}\right)_V-P.}
$$

For equilibrium radiation, $E=Ve(T)$ and $P=e(T)/3$, so this identity reads $e=Te'/3-e/3$, or $Te'=4e$. Integrating gives

$$
\boxed{e=aT^4,\qquad E=aVT^4.}
$$

Finally in a reversible adiabatic expansion, $dE=-P\,dV$ becomes $4aVT^3dT+aT^4dV=-aT^4dV/3$. Dividing gives $3\,dT/T=-dV/V$, hence **$VT^3$ is constant**. This assumes equilibrium radiation throughout the expansion.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
