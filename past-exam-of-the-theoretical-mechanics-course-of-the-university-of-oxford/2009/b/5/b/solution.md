<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\widehat\eta(k,t)=\int\eta(x,t)e^{-ikx}\,dx$ and the inverse factor $1/(2\pi)$. Fourier transformation gives $\widehat\eta_{tt}+\lambda^2k^4\widehat\eta=0$. The supplied Lorentzian transform and zero initial [velocity](../../../../../velocity.md) therefore imply

$$
\boxed{\widehat\eta=ae^{-\epsilon|k|}\cos(\lambda k^2t),\qquad\eta(x,t)=\frac1{2\pi}\int\widehat\eta(k,t)e^{ikx}\,dk.}
$$

Along $x=Vt$, split the cosine into two exponentials. Their phases are $\psi_\pm=Vk\pm\lambda k^2$, with stationary points $k_\pm=\mp V/(2\lambda)$, phase values $\mp V^2/(4\lambda)$ and second derivatives $\pm2\lambda$. Both amplitudes equal $ae^{-\epsilon|V|/(2\lambda)}$. The two stationary-phase contributions are conjugate, giving

$$
\boxed{\eta(Vt,t)=\frac{ae^{-\epsilon|V|/(2\lambda)}}{2\sqrt{\pi\lambda t}}\cos\left(\frac{V^2t}{4\lambda}-\frac\pi4\right)+o(t^{-1/2}).}
$$

Thus the finite-width pulse retains a ray-dependent attenuation. In the further regime $\epsilon|V|/(2\lambda)\ll1$, it may be replaced by one, recovering

$$
\boxed{\eta(x,t)\sim\frac{a}{2\sqrt{\pi\lambda t}}\cos\left(\frac{x^2}{4\lambda t}-\frac\pi4\right).}
$$

The large-time ray limit means $V=x/t$ is fixed. Merely making both $x$ and $t$ large does not justify dropping the attenuation if $|x|/t$ becomes large compared with $\lambda/\epsilon$. The leading oscillation decays as $t^{-1/2}$ because each saddle samples a Fourier band of width $t^{-1/2}$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
