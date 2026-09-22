<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $E>0$, put $k=\sqrt{2mE}$ and $q=k/\hbar>0$. Outside the support of the [potential energy](../../../../potential-energy.md), a [generalized eigenfunction](../../../../generalized-eigenfunction.md) of the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) has the [plane wave](../../../../plane-wave.md) form

$$
\psi(x)=\begin{cases}A e^{iqx}+B e^{-iqx},&x<-R_0,\\C e^{iqx}+D e^{-iqx},&x>R_0.\end{cases}
$$

Here $R_0$ denotes the support radius, to distinguish it from the [quantum reflection probability](../../../../quantum-reflection-probability.md) $R$. The [momenta](../../../../momentum-split.md) are $\pm k$ and the [velocities](../../../../velocity.md) are $\pm k/m$. Thus $A,D$ describe incoming [scattering channels](../../../../scattering-channel.md) from the left and right, and $B,C$ describe outgoing [scattering channels](../../../../scattering-channel.md) towards the left and right. These [energy eigenfunctions](../../../../energy-eigenfunction.md) are not [square-integrable functions](../../../../square-integrable-function.md); normalizable incoming [wave packets](../../../../wave-packet.md) are formed by superposition over [energy](../../../../energy-split.md), and their passage through the interaction region gives the physical [quantum scattering](../../../../quantum-scattering-split.md) experiment.

For incidence from the left, normalize $A=1,D=0$ and write $B=r_L,C=t_L$. The [quantum reflection amplitude](../../../../quantum-reflection-amplitude.md) is $r_L$ and the [transmission amplitude](../../../../transmission-amplitude.md) is $t_L$. The ratios of outgoing to incident [probability currents](../../../../probability-current.md) define

$$
\boxed{R=|r_L|^2,\qquad T=|t_L|^2.}
$$

No extra [velocity](../../../../velocity.md) ratio occurs because both exterior regions have the same [potential energy](../../../../potential-energy.md) and [mass](../../../../mass.md). The [scattering matrix](../../../../s-matrix.md), with a fixed choice of channel order, is

$$
\boxed{\begin{pmatrix}B\\C\end{pmatrix}=S(q)\begin{pmatrix}A\\D\end{pmatrix},\qquad S(q)=\begin{pmatrix}r_L&t_R\\t_L&r_R\end{pmatrix}.}
$$

Its first and second columns are the responses to unit incidence from the left and right, respectively. For a reflection-symmetric [potential energy](../../../../potential-energy.md), these conventions give $r_L=r_R=r$ and $t_L=t_R=t$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
