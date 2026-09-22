# Three-neuron ring stability

↑ **Parent:** [Computational neuroscience](computational-neuroscience.md)

For a directed three-neuron rate ring $\tau\dot x_i=-x_i+W_{i,i-1}\tanh(\beta x_{i-1})$, the linearization has characteristic equation $(1+\tau\lambda)^3=\Gamma$, where $\Gamma=\beta^3W_{13}W_{32}W_{21}$. Positive loop gain has strict linear asymptotic stability for $\Gamma<1$. Negative loop gain has it for $-8<\Gamma<0$; at $\Gamma=-8$ a complex pair crosses the imaginary axis at frequency $\sqrt3/\tau$. The saturating cubic gives a [supercritical Hopf bifurcation](supercritical-hopf-bifurcation.md) under an ordinary loop-gain variation. This directed system does not inherit the energy-descent property of a symmetric [Hopfield network](hopfield-network.md).

## ↑ Ancestors (4)

1. [Computational neuroscience](computational-neuroscience.md)
2. [Neuroscience](neuroscience.md)
3. [Biology](biology-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/c/solution.md)
