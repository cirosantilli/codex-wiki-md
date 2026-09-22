<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real angles write $u_p=\cos\theta_p$ and $v_p=\sin\theta_p$. For one independent pair $p>0$, the transformation and its conjugate read

$$
c_p=u_p\alpha_p+i v_p\alpha_{-p}^\dagger,\qquad
c_{-p}=u_p\alpha_{-p}-i v_p\alpha_p^\dagger.
$$

Using the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) for the $\alpha$ modes gives

$$
\begin{aligned}
\{c_p,c_p^\dagger\}&=u_p^2+v_p^2=1,\\
\{c_{-p},c_{-p}^\dagger\}&=u_p^2+v_p^2=1,\\
\{c_p,c_{-p}\}&=-i u_pv_p+i v_pu_p=0,\\
\{c_p,c_{-p}^\dagger\}&=0.
\end{aligned}
$$

The remaining [anticommutators](../../../../anticommutator.md) vanish for independent [momentum](../../../../momentum-split.md) pairs. The displayed two-by-two [matrix](../../../../matrix.md) is [unitary](../../../../unitary-connection.md) and its inverse is obtained by changing $i$ to $-i$.

When the same formula is indexed over both signs of [momentum](../../../../momentum-split.md), its first row at $-p$ must agree with the conjugate of its second row at $p$. Thus a consistent global convention requires

$$
\boxed{u_{-p}=u_p,\qquad v_{-p}=-v_p,\qquad \theta_{-p}=-\theta_p\pmod{2\pi}.}
$$

This is the [odd-momentum fermionic Bogoliubov angle](../../../../odd-momentum-fermionic-bogoliubov-angle.md) convention. If one checks only the first-row formulas, their cross [anticommutator](../../../../anticommutator.md) is $i\sin(\theta_p+\theta_{-p})$; its vanishing gives the condition modulo $\pi$, with possible signs absorbable in the $\alpha$ modes. Requiring both rows to describe the same operators fixes the convention above. Merely checking a separate [unitary matrix](../../../../unitary-matrix.md) at each [momentum](../../../../momentum-split.md) misses this redundancy: choosing $\theta_p=\theta_{-p}=\pi/4$ in both first rows would give $\{c_p,c_{-p}\}=i$.

At $p=0$, the [annihilation operator](../../../../annihilation-operator.md) and its conjugate belong to one mode. The full displayed formula is consistent only with $v_0=0$; choose $\theta_0=0$ and $\alpha_0=c_0$. This mode is not a two-mode pair.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
