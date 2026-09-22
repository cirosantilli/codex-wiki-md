<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the sense of rotation by taking the fluid [velocity](../../../../../../velocity.md) to be $\mathbf u=\Omega(-x_3,0,x_1)$, with $\Omega>0$. Its [vorticity](../../../../../../vorticity.md) is $-2\Omega\mathbf e_2$. In the convention where $B$ is the [gyrotactic reorientation time](../../../../../../gyrotactic-reorientation-time.md) appearing with aligning rate $1/B$, the [bottom-heavy spherical-cell orientation dynamics](../../../../../../bottom-heavy-spherical-cell-orientation-dynamics.md) is

$$
\dot{\mathbf p}=\frac1B(\mathbf e_3-p_3\mathbf p)-\Omega\mathbf e_2\times\mathbf p.
$$

For the stable orientation in the transverse plane, write $\mathbf p=(\sin\vartheta,0,\cos\vartheta)$. The angle equation is $\dot\vartheta=-\sin\vartheta/B-\Omega$. If $B\Omega<1$, its stable fixed point satisfies

$$
\sin\vartheta_*=-B\Omega,\qquad\cos\vartheta_*=\sqrt{1-B^2\Omega^2},\qquad
\boxed{\mathbf p_*=(-B\Omega,0,\sqrt{1-B^2\Omega^2}).}
$$

The other planar fixed point has negative $p_3$ and is unstable. The positive-$p_3$ orientation also damps a small out-of-plane component because $\dot p_2=-p_3p_2/B$.

Once the orientation has relaxed to $\mathbf p_*$, the transverse trajectory obeys

$$
\dot x_1=-\Omega x_3-V_sB\Omega,\qquad
\dot x_3=\Omega x_1+V_s\sqrt{1-B^2\Omega^2}.
$$

Define the shifted axis by

$$
\boxed{x_{1A}=-\frac{V_s}{\Omega}\sqrt{1-B^2\Omega^2},\qquad x_{3A}=-V_sB.}
$$

Then $(x_1-x_{1A},x_3-x_{3A})$ rotates rigidly with angular speed $\Omega$, so its squared length is constant. These are the [gyrotactic circular paths in a rotating cylinder](../../../../../../gyrotactic-circular-paths-in-a-rotating-cylinder.md), and

$$
\boxed{|OA|=\frac{V_s}{\Omega},\qquad \alpha=\arcsin(B\Omega).}
$$

Here $\alpha$ is the acute angle between the plane through the two parallel axes and the horizontal plane; the directed displacement $OA$ in the chosen cross-section points to the lower-left. Reversing the sense of rotation reverses the horizontal displacement. Arbitrary initial orientations have an orientation transient before the exact circular trajectories; neglecting randomness alone does not remove that transient. The bulk result also assumes that the trajectory does not intersect the cylinder wall.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
