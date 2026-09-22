<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The component distances from the [centre of mass](../../../../../center-of-mass.md) are $a_1=aM_2/M$ and $a_2=aM_1/M$, where $M=M_1+M_2$. Their orbital angular momenta add to

$$
\begin{aligned}
J
&=M_1a_1^2\Omega+M_2a_2^2\Omega\\
&=\boxed{\frac{M_1M_2}{M}a^2\Omega}.
\end{aligned}
$$

Let $W>0$ be the isotropic wind-loss magnitude, so $\dot M_1=-W$ and $\dot M_2=0$. The wind carries star 1's specific orbital angular momentum $j_1=a_1^2\Omega$, and hence

$$
\frac{\dot J}{J}
=-W\frac{j_1}{J}
=-W\frac{M_2}{M_1M}.
$$

Using [Kepler third law](../../../../../kepler-s-third-law.md) to write $J=M_1M_2\sqrt{Ga/M}$ and differentiating shows

$$
\frac{\dot a}{a}=\frac{W}{M},
\qquad
\boxed{aM=\text{constant}}.
$$

Since $P^2\propto a^3/M$, it follows that

$$
\boxed{PM^2=\text{constant}}.
$$

This is [Jeans-mode mass loss](../../../../../jeans-mode-mass-loss.md).

Now allow transfer to star 2 at rate $\dot M_2>0$ while the wind continues. Then

$$
\dot M_1=-W-\dot M_2,
\qquad
\dot M_{\rm total}=-W.
$$

The same [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) calculation gives

$$
\frac{\dot a}{a}
=\frac{W}{M}
+2\dot M_2\left(\frac1{M_1}-\frac1{M_2}\right).
$$

The donor response $R\propto M_1^{-n}$ is

$$
\frac{\dot R}{R}=n\frac{W+\dot M_2}{M_1},
$$

while

$$
\frac{\dot R_L}{R_L}
=\frac{\dot a}{a}
+\frac13\left(\frac{\dot M_1}{M_1}
-\frac{\dot M_{\rm total}}M\right).
$$

Before contact, put $\dot M_2=0$. The wind drives the star farther into its [Roche lobe](../../../../../roche-lobe.md) when $\dot{\log}(R/R_L)>0$. With $q=M_1/M_2$, this condition reduces to

$$
\boxed{q<\frac{1+3n}{3(1-n)}}.
$$

If the inequality is reversed, the Roche lobe expands relative to the donor, so wind loss detaches the star and no wind-driven Roche-lobe transfer is sustained; later nuclear expansion may restore contact.

During stable contact, impose $\dot R/R=\dot R_L/R_L$ and solve for the transfer rate. Straightforward algebra gives

$$
\boxed{\dot M_2
=\frac{1+3n-3(1-n)q}
{(1+q)(5-3n-6q)}\,W}.
$$

In the paper's signed notation $W=-\dot M$, this is exactly

$$
\boxed{\dot M_2
=-\frac{1+3n-3(1-n)q}
{(1+q)(5-3n-6q)}\,\dot M}.
$$

If

$$
5-3n-6q<0,
$$

the stationary response has the wrong sign: transfer enlarges the overfill rather than removing it. [Dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) is lost, leading to runaway transfer and usually a [common envelope](../../../../../common-envelope.md) or merger.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
