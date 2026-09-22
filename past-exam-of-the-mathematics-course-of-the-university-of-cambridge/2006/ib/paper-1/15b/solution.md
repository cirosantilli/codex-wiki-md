<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

**No: ordering the attractive potentials does not impose the proposed ordering of reflection probabilities.** Take $k=\pi/(4a)$ and let $M$ denote the particle mass. Choose $V_2=0$ everywhere and

$$
V_1(x)=\begin{cases}-4\hbar^2k^2/M,&|x|<a,\\0,&|x|\ge a.\end{cases}
$$

These satisfy every stated ordering and support condition. The incoming energy is $\hbar^2k^2/(2M)$; the interior [wavenumber](../../../../../wavenumber.md) in the [finite square well](../../../../../finite-square-well.md) is $q=\sqrt{k^2-2MV_1/\hbar^2}=3k$.

Here is an explicit matching calculation. For a general well of width $L=2a$, take exterior waves $e^{ik(x+a)}+re^{-ik(x+a)}$ on the left and $te^{ik(x-a)}$ on the right. Shifting the incident phase in this way does not change the [reflection probability](../../../../../quantum-reflection-probability.md). Continuity of the [wavefunction](../../../../../wave-function.md) and its first [derivative](../../../../../derivative.md) gives the propagation relation

$$
\begin{pmatrix}t\\ikt\end{pmatrix}
=\begin{pmatrix}\cos(qL)&\sin(qL)/q\\-q\sin(qL)&\cos(qL)\end{pmatrix}
\begin{pmatrix}1+r\\ik(1-r)\end{pmatrix}.
$$

Inverting it and adding the two equations after dividing the [derivative](../../../../../derivative.md) equation by $ik$ yields

$$
t=\frac2{2\cos(qL)-i(k/q+q/k)\sin(qL)},\qquad
r=\frac{i(q/k-k/q)\sin(qL)}{2\cos(qL)-i(k/q+q/k)\sin(qL)}.
$$

The incident and reflected exterior waves have the same speed, so their [flux](../../../../../flux.md) ratio is

$$
p_1=|r|^2=\frac{(q^2-k^2)^2\sin^2(qL)}{4k^2q^2+(q^2-k^2)^2\sin^2(qL)}.
$$

For the chosen parameters $qL=3\pi/2$ and $(q^2-k^2)^2/(4k^2q^2)=16/9$. Thus

$$
\boxed{p_1=\frac{16}{25},\qquad p_2=0.}
$$

The zero potential has no reflected component. This proves the failure with explicit probabilities. More generally the same expression vanishes at $qL\in\pi\mathbb Z$, explaining [resonant transmission through a square well](../../../../../resonant-transmission-through-a-square-well.md) and why increasing attractive well depth does not monotonically control reflection.

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
