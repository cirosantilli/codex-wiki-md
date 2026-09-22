<h1 id="38a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The physical rapid phase is

$$
\Theta(\mathbf x,t)=\frac{\theta(\mathbf x,t)}{\varepsilon}.
$$

Define the local [wavevector](../../../../../../wavevector.md), [angular frequency](../../../../../../angular-frequency.md), and [group velocity](../../../../../../group-velocity.md) by

$$
k_i=\frac{\partial\Theta}{\partial x_i}
=\frac1\varepsilon\frac{\partial\theta}{\partial x_i},
\qquad
\omega=-\frac{\partial\Theta}{\partial t}
=-\frac1\varepsilon\frac{\partial\theta}{\partial t},
\qquad
c_{g,i}=\frac{\partial\Omega}{\partial k_i}.
$$

The equality of mixed partial derivatives gives the phase-compatibility equations

$$
\frac{\partial k_i}{\partial t}
+\frac{\partial\omega}{\partial x_i}=0,
\qquad
\frac{\partial k_i}{\partial x_j}
=\frac{\partial k_j}{\partial x_i}.
$$

A ray is defined to move with the local group velocity:

$$
\boxed{\frac{dx_i}{dt}=\frac{\partial\Omega}{\partial k_i}.}
$$

Differentiate the local [dispersion relation](../../../../../../dispersion-relation.md)

$$
\omega=\Omega(\mathbf k;\mathbf x,t)
$$

with respect to $x_i$. Along a ray,

$$
\begin{aligned}
\frac{dk_i}{dt}
&=\frac{\partial k_i}{\partial t}
+\frac{dx_j}{dt}\frac{\partial k_i}{\partial x_j}\\
&=-\frac{\partial\omega}{\partial x_i}
+\frac{\partial\Omega}{\partial k_j}
\frac{\partial k_i}{\partial x_j}\\
&=-\frac{\partial\Omega}{\partial x_i}
-\frac{\partial\Omega}{\partial k_j}
\frac{\partial k_j}{\partial x_i}
+\frac{\partial\Omega}{\partial k_j}
\frac{\partial k_i}{\partial x_j}\\
&=-\frac{\partial\Omega}{\partial x_i}.
\end{aligned}
$$

The last two terms cancel because $\mathbf k$ is a [gradient](../../../../../../gradient.md). Similarly,

$$
\begin{aligned}
\frac{d\omega}{dt}
&=\frac{\partial\Omega}{\partial t}
+\frac{\partial\Omega}{\partial x_i}\frac{dx_i}{dt}
+\frac{\partial\Omega}{\partial k_i}\frac{dk_i}{dt}\\
&=\frac{\partial\Omega}{\partial t}.
\end{aligned}
$$

Finally,

$$
\frac1\varepsilon\frac{d\theta}{dt}
=\frac{\partial\Theta}{\partial t}
+\frac{dx_j}{dt}\frac{\partial\Theta}{\partial x_j}
=-\omega+k_j\frac{\partial\Omega}{\partial k_j}.
$$

Thus the [Hamiltonian ray-tracing equations](../../../../../../hamiltonian-ray-tracing-equations.md) are

$$
\boxed{
\frac{dx_i}{dt}=\frac{\partial\Omega}{\partial k_i},
\qquad
\frac{d\omega}{dt}=\frac{\partial\Omega}{\partial t},
\qquad
\frac{dk_i}{dt}=-\frac{\partial\Omega}{\partial x_i},
\qquad
\frac1\varepsilon\frac{d\theta}{dt}
=-\omega+k_j\frac{\partial\Omega}{\partial k_j}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38A](../../38a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
