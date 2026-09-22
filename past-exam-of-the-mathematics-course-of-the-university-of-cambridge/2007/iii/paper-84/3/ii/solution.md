<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the central [number density](../../../../../../number-density.md) $n_c$, radius $R$ and central [healing length](../../../../../../healing-length.md) $\xi$ from the preceding part. The vortex energy means the excess over the no-vortex ground state at fixed particle number. Choose an intermediate matching radius $\xi\ll L\ll R$. Inside $L$, the trapped [number density](../../../../../../number-density.md) differs little from $n_c$, so the resolved uniform vortex core gives

$$
\Delta E_{\rm inner}\simeq\frac{\pi n_c\hbar^2}{m}
\left[\log\frac L\xi+L_{01}\right].
$$

Outside the core, the singly quantized [superfluid velocity](../../../../../../superfluid-velocity.md) is $u_\theta=\hbar/(mr)$. Its leading flow [kinetic energy](../../../../../../kinetic-energy.md) in the parabolic background is therefore

$$
\begin{aligned}
\Delta E_{\rm outer}
&\simeq\frac12\int_L^R m n_{\rm TF}(r)u_\theta^2\,2\pi r\,dr\\
&=\frac{\pi n_c\hbar^2}{m}\int_L^R\left(1-\frac{r^2}{R^2}\right)\frac{dr}{r}\\
&=\frac{\pi n_c\hbar^2}{m}\left[\log\frac RL-\frac12+\frac{L^2}{2R^2}\right].
\end{aligned}
$$

Adding the regions cancels the arbitrary matching radius. Sending $L/R\to0$ while $\xi/L\to0$ gives the [matched vortex energy in a parabolic condensate](../../../../../../matched-vortex-energy-in-a-parabolic-condensate.md)

$$
\boxed{\Delta E_1\simeq\frac{\pi n_c\hbar^2}{m}
\left[\log\frac R\xi+L_{01}-\frac12\right]
=\frac{2N\hbar^2}{mR^2}\left[\log\frac R\xi+L_{01}-\frac12\right]}.
$$

The $-1/2$ comes from the decrease of background [number density](../../../../../../number-density.md) away from the centre. It would be missed by treating the whole trap as uniform. To this accuracy, using the unperturbed TF density in the outer region is appropriate at fixed $N$: the first variation of trapping plus interaction energy is $\mu\,\delta N$ and therefore vanishes after the small normalization adjustment. The resolved core energy supplies the finite core correction $L_{01}$, while remaining cloud-edge and density-relaxation corrections vanish in the small-core TF limit. This is an asymptotic energy estimate, not an exact formula at finite $R/\xi$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
