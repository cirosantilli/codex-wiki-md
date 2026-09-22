<h1 id="40d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use complex fields with time factor $e^{i\omega t}$ and put $k_\pm=\omega/c_\pm$. The outgoing potential in $x>0$ is

$$
\Phi_+(x)=T e^{-ik_+x}.
$$

Continuity of [pressure](../../../../../../../pressure.md) and [velocity](../../../../../../../velocity.md) at $x=0$ gives

$$
\Phi_-(0)=\frac{\rho_+}{\rho_-}T,
\qquad
\Phi_-'(0)=-ik_+T.
$$

Hence

$$
\Phi_-(x)=T\left[
\frac{\rho_+}{\rho_-}\cos(k_-x)
-i\frac{c_-}{c_+}\sin(k_-x)
\right].
$$

The piston condition $\Phi_-'(-L)=i\omega\epsilon$, with $\lambda=k_-L$, gives

$$
\boxed{
T=\epsilon c_-
\frac{i(\rho_+/\rho_-)\sin\lambda-(c_-/c_+)\cos\lambda}
 { (\rho_+/\rho_-)^2\sin^2\lambda+(c_-/c_+)^2\cos^2\lambda}.}
$$

This is the [transmitted velocity potential from a piston through an acoustic interface](../../../../../../../transmitted-velocity-potential-from-a-piston-through-an-acoustic-interface.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [40D](../../../40d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
