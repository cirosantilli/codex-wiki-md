<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For homogeneous corrections at the square boundary, [integration by parts](../../../../../../integration-by-parts.md) gives $\langle\psi_0\Delta\psi_1\rangle=\langle\psi_1\Delta\psi_0\rangle$ and $\langle\theta_0\Delta\theta_1\rangle=\langle\theta_1\Delta\theta_0\rangle$. The first-derivative cross terms give $\langle\psi_0\theta_{1x}\rangle=-\langle\psi_{0x}\theta_1\rangle$ and $\langle\theta_0\psi_{1x}\rangle=-\langle\theta_{0x}\psi_1\rangle$. Using $\Delta\psi_0=q_c^2\theta_{0x}$ and $\Delta\theta_0=-\psi_{0x}$, these four contributions cancel in pairs. This proves exactly the supplied [solvability condition](../../../../../../solvability-condition.md), including the weight $q_c^2$ on its second row. Equivalently $(\psi_0,q_c^2\theta_0)$ is the relevant [adjoint eigenfunction](../../../../../../adjoint-eigenfunction.md) for this coupled system.

At first order in the detuning, the inhomogeneous equations are

$$
\Delta\psi_1-q_c^2\theta_{1x}=2q_cq_1\theta_{0x},\qquad \psi_{1x}+\Delta\theta_1=\lambda\theta_0.
$$

Insert these right-hand sides into the verified [solvability condition](../../../../../../solvability-condition.md). One obtains

$$
2q_cq_1\langle\psi_0\theta_{0x}\rangle+q_c^2\lambda\langle\theta_0^2\rangle=0.
$$

A further [integration by parts](../../../../../../integration-by-parts.md), using the leading [heat equation](../../../../../../heat-equation.md), gives

$$
\langle\psi_0\theta_{0x}\rangle=-\langle\psi_{0x}\theta_0\rangle=\langle\theta_0\Delta\theta_0\rangle=-\langle|\nabla\theta_0|^2\rangle.
$$

Hence the [growth-rate solvability for conducting-square Darcy convection](../../../../../../growth-rate-solvability-for-conducting-square-darcy-convection.md) yields

$$
\boxed{\lambda=\frac{2q_1}{q_c}\frac{\langle|\nabla\theta_0|^2\rangle}{\langle\theta_0^2\rangle}.}
$$

**The PDF prints the reciprocal of the required integral ratio.** With its declared $\theta_t=\epsilon\lambda\theta$, the displayed reciprocal does not follow and is false for $q_1\neq0$. Both integrals are positive for these nonzero modes. The square's [Poincaré inequality](../../../../../../poincare-inequality.md) gives their ratio at least $2\pi^2$, so it cannot equal its reciprocal. For $q_1=1$, the two explicit parities give approximately $\lambda=11.34770$ for odd $\theta$ and $\lambda=7.30164$ for even $\theta$; the printed expression instead gives about $0.00446439$ and $0.00693825$. These values provide direct mode-based counterexamples.

The corrected growth rate is positive for $q_1>0$ and negative for $q_1<0$, as expected at a [convection](../../../../../../convection.md) threshold. Because the critical [eigenspace](../../../../../../eigenspace.md) is two-dimensional, an arbitrary superposition generally splits into two different first-order growth rates. The specified parity modes remain independent under the detuning: the [temperature](../../../../../../temperature.md) [linear operator](../../../../../../linear-operator.md) preserves reflection parity, so the cross-parity projection vanishes. This justifies applying the scalar [solvability condition](../../../../../../solvability-condition.md) to either listed [eigenfunction](../../../../../../eigenfunction.md); it should not be applied as a single common [eigenvalue](../../../../../../eigenvalue.md) to an arbitrary mixture.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
