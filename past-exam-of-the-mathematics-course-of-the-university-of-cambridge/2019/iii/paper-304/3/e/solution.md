<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Restore the dimensional-regularization factor $\mu^\epsilon$ and define

$$
N_0=2i(1-x)\not p+4m,
\qquad N_1=i(1-x)\not p+m.
$$

Using $\Gamma(\epsilon/2)=2/\epsilon-\gamma+O(\epsilon)$ gives

$$
\boxed{\Sigma(\not p)=-\frac{e^2}{16\pi^2}\int_0^1dx
\left\{
\frac{2N_0}{\epsilon}
+N_0\left[\log\frac{4\pi\mu^2}{\Delta}-\gamma\right]
-2N_1
\right\}+O(\epsilon).}
$$

The first term is the [ultraviolet divergence](../../../../../../ultraviolet-divergence.md). In the [modified minimal subtraction scheme](../../../../../../modified-minimal-subtraction-scheme.md), subtraction of $2/\epsilon-\gamma+\log4\pi$ leaves

$$
\Sigma_{\overline{\rm MS}}(\not p)
=-\frac{e^2}{16\pi^2}\int_0^1dx
\left[N_0\log\frac{\mu^2}{\Delta}-2N_1\right].
$$

On the tree-level mass shell, $p^2=-m^2$ and $i\not p=-m$, so $\Delta=x^2m^2$. The [mass counterterm](../../../../../../mass-counterterm.md) is

$$
\boxed{\delta m_{\overline{\rm MS}}
=-\frac{3e^2m}{16\pi^2}
\left(\frac2\epsilon-\gamma+\log4\pi\right).}
$$

The pole condition $m_{\rm phys}=m-\Sigma_{\overline{\rm MS}}|_{i\not p=-m}+O(e^4)$ therefore gives

$$
\boxed{m_{\rm phys}=m(\mu)\left[
1+\frac{e^2}{8\pi^2}\int_0^1dx
\left((1+x)\log\frac{\mu^2}{x^2m^2}-x\right)
\right]+O(e^4).}
$$

Evaluating the elementary parameter integral yields the equivalent expression

$$
m_{\rm phys}=m(\mu)\left[1+\frac{e^2}{4\pi^2}
\left(1+\frac34\log\frac{\mu^2}{m^2}\right)\right]+O(e^4).
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
