<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume constant current, $g_L>0$, $C_m>0$, and reset below threshold. With $g_E=0$, $V_\infty=V_L+I_e/g_L$. A spike occurs in finite time after reset precisely when $V_\infty>V_\theta$, so the critical boundary is

$$
\boxed{I_c=g_L(V_\theta-V_L)}.
$$

At equality the voltage approaches threshold asymptotically, so the finite-time firing condition is the strict inequality $I_e>I_c$.

Solve the exponential voltage trajectory from reset to threshold. The interspike interval of this [constant-input firing rate of a leaky integrate-and-fire neuron](../../../../../../constant-input-firing-rate-of-a-leaky-integrate-and-fire-neuron.md) is

$$
T=\frac{C_m}{g_L}\log\frac{V_\infty-V_0}{V_\infty-V_\theta}=\frac{C_m}{g_L}\log\left(1+\frac{g_L(V_\theta-V_0)}{I_e-I_c}\right).
$$

Thus

$$
\boxed{r(I_e)=0\ (I_e\leq I_c),\qquad r(I_e)=T^{-1}\ (I_e>I_c)}.
$$

The logarithm decreases strictly with current, so $r$ increases, starting from zero as $I_e\downarrow I_c$. At large current, its argument increment is small and

$$
T\sim\frac{C_m(V_\theta-V_0)}{I_e-I_c},\qquad\boxed{r(I_e)\sim\frac{I_e}{C_m(V_\theta-V_0)}}.
$$

The second expression states the leading linear growth, not an exact intercept formula. If an explicit refractory time $t_{\rm ref}$ is added, the rate instead becomes $1/(T+t_{\rm ref})$ and approaches $1/t_{\rm ref}$ at very high current. The printed model contains no such extra interval, which is why its unrestricted high-current rate is linear.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
