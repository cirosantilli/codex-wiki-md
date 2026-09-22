# RF-averaged trapping potential

↑ **Parent:** [Paul trap](paul-trap.md)

Write the RF [electric field](electric-field-split.md) as $\mathbf E_{\rm amp}(\mathbf r)\cos\Omega t$, where $\mathbf E_{\rm amp}$ is a real peak-amplitude vector with a common drive phase. Decompose the trajectory into a slow position $\mathbf R$ and fast displacement $\boldsymbol\xi$. Over one short RF cycle, hold $\mathbf R$ fixed. The leading fast equation and solution are

$$
m\ddot{\boldsymbol\xi}=Q\mathbf E_{\rm amp}(\mathbf R)\cos\Omega t,\qquad
\boldsymbol\xi=-\frac{Q\mathbf E_{\rm amp}(\mathbf R)}{m\Omega^2}\cos\Omega t.
$$

The homogeneous slow part is absorbed into $\mathbf R$. Expand the [electric field](electric-field-split.md) to first order in $\boldsymbol\xi$ and average, using $\langle\cos^2\Omega t\rangle=1/2$:

$$
\langle\mathbf F\rangle=-\frac{Q^2}{2m\Omega^2}(\mathbf E_{\rm amp}\cdot\nabla)\mathbf E_{\rm amp}
=-\nabla\left(\frac{Q^2|\mathbf E_{\rm amp}|^2}{4m\Omega^2}\right).
$$

The second equality uses zero [curl](curl.md) in the quasistatic RF [electric field](electric-field-split.md). This derives an effective [potential energy](potential-energy.md), not an extra static [electric potential](electric-potential.md). Its $Q^2$ dependence confines either sign of [electric charge](electric-charge-split.md) towards a field-amplitude minimum. Using an RMS field instead would give a coefficient $1/(2m\Omega^2)$ multiplying $Q^2|\mathbf E_{\rm rms}|^2$.

The approximation needs fast displacement small compared with the field's variation length and slow [angular frequencies](angular-frequency.md) small compared with $\Omega$. In the stated [electric quadrupole](electric-quadrupole.md) model, small $|q_i|$ and $a_i$ of order $q_i^2$ provide a controlled regime, away from stability boundaries. Add $Q\Phi_{\rm dc}$ when $U\ne0$. For $U=0$ the result is

$$
U_{\rm eff}=\frac{Q^2V^2}{4m\Omega^2d^4}(x^2+y^2+4z^2),\qquad
\omega_i\simeq\frac{\Omega}{2}\sqrt{a_i+\frac{q_i^2}{2}}.
$$

For the pure RF case, $\omega_z\simeq2\omega_x=2\omega_y$. The square-root condition describes leading local restoring curvature; it is not a substitute for full [Mathieu equation](mathieu-equation.md) stability. Collisions, departures from the ideal [electric quadrupole](electric-quadrupole.md), and a displaced RF null require further analysis.

## ↑ Ancestors (6)

1. [Paul trap](paul-trap.md)
2. [Ion trap](ion-trap.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Paul trap](paul-trap.md)
- [Paul trap micromotion](paul-trap-micromotion.md)
- [Paul trap secular motion](paul-trap-secular-motion.md)
- [Trapped-ion quantum control](trapped-ion-quantum-control.md)
