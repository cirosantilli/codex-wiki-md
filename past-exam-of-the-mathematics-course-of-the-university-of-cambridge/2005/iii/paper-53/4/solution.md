<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An antilinear involution need not preserve norms, so the required physical assumption is that momentum reversal maps a complete normalized basis to a normalized basis. For a spinless sector take $\hat T|\boldsymbol p\rangle=\eta(\boldsymbol p)|-\boldsymbol p\rangle$ with $|\eta|=1$ and relativistic normalization $\langle\boldsymbol p|\boldsymbol q\rangle=(2\pi)^3 2E_p\delta^3(\boldsymbol p-\boldsymbol q)$. Any extra degeneracy labels must likewise be mapped by a norm-preserving permutation or unitary matrix. The condition $\hat T^2=1$ requires $\eta(-\boldsymbol p)\eta(\boldsymbol p)^*=1$ in the scalar basis.

For arbitrary normalizable wave packets $|\phi\rangle=\int d\Pi_p\,f(\boldsymbol p)|\boldsymbol p\rangle$ and $|\psi\rangle=\int d\Pi_p\,h(\boldsymbol p)|\boldsymbol p\rangle$, where $d\Pi_p=d^3p/[(2\pi)^3 2E_p]$, antilinearity conjugates their coefficients. Using the normalized reversed basis gives

$$
\langle\hat T\phi|\hat T\psi\rangle=\int d\Pi_p\,f(\boldsymbol p)h(\boldsymbol p)^*|\eta(\boldsymbol p)|^2
=\left[\int d\Pi_p\,f(\boldsymbol p)^*h(\boldsymbol p)\right]^*.
$$

Completeness proves **$\langle\hat T\phi|\hat T\psi\rangle=\langle\phi|\psi\rangle^*$ for all states**, so this [quantum time-reversal operator](../../../../../quantum-time-reversal-operator.md) is [antiunitary](../../../../../antiunitary-operator.md). The same proof with sums over extra labels uses the unitarity of their reversal matrix.

For a Hermitian interaction-picture Hamiltonian, the condition of [time-reversal symmetry](../../../../../t-symmetry.md) is

$$
\boxed{\hat TV(t)\hat T^{-1}=V(-t),\qquad V(t)^\dagger=V(t).}
$$

Expand the [scattering matrix](../../../../../s-matrix.md) as a [Dyson series](../../../../../dyson-series.md), using ordered integration rather than commuting operators:

$$
S=1+\sum_{n\geq1}(-i)^n\int_{t_1>\cdots>t_n}dt_1\cdots dt_n\,V(t_1)\cdots V(t_n).
$$

Conjugation by $\hat T$ conjugates $(-i)^n$ to $i^n$ but preserves the product order. Substitute $s_j=-t_j$; the integration domain becomes $s_1<\cdots<s_n$ and

$$
\hat TS\hat T^{-1}=1+\sum_{n\geq1}i^n\int_{s_1<\cdots<s_n}ds_1\cdots ds_n\,V(s_1)\cdots V(s_n).
$$

On the other hand, taking the adjoint of the original series conjugates its coefficient and reverses the operator order. Relabel $s_1=t_n,\ldots,s_n=t_1$ in each adjoint integral; it is exactly the same series. Thus

$$
\boxed{\hat TS\hat T^{-1}=S^\dagger.}
$$

Equivalently, [time ordering](../../../../../time-ordering.md) turns into anti-[time ordering](../../../../../time-ordering.md) after reversing the time arguments. One can first use a finite symmetric time interval and the same time-symmetric switching prescription before taking the scattering limit; the argument never assumes $[V(t),V(s)]=0$.

[Antiunitarity](../../../../../antiunitary-operator.md) relates amplitudes by

$$
\langle\hat Tf|\hat TS\hat T^{-1}|\hat Ti\rangle=\langle f|S|i\rangle^*.
$$

Using $\hat TS\hat T^{-1}=S^\dagger$ and taking a complex conjugate gives the [time-reversal reciprocity of the scattering matrix](../../../../../time-reversal-reciprocity-of-the-scattering-matrix.md)

$$
\boxed{\langle f|S|i\rangle=\langle\hat Ti|S|\hat Tf\rangle.}
$$

The reverse process starts with the reversed final state and ends with the reversed initial state. Intrinsic state phases can appear when these reversed states are rewritten in a separately chosen basis, but the corresponding squared amplitudes agree. Equal amplitudes do not mean identical numerical cross sections when the reversed process has different flux or phase-space factors.

For a [spin](../../../../../spin.md)-zero [complex scalar field](../../../../../complex-scalar-field.md), choose the transformation convention $\hat T\phi(t,\boldsymbol x)\hat T^{-1}=\eta_T\phi(-t,\boldsymbol x)$. Its [mode expansion of a free field](../../../../../mode-expansion-of-a-free-field.md) is

$$
\phi(t,\boldsymbol x)=\int d\Pi_p\left[a(\boldsymbol p)e^{-iE_pt+i\boldsymbol p\cdot\boldsymbol x}
+b^\dagger(\boldsymbol p)e^{iE_pt-i\boldsymbol p\cdot\boldsymbol x}\right].
$$

Apply $\hat T$ to the expansion. Its [antiunitarity](../../../../../antiunitary-operator.md) conjugates both numerical plane waves, giving coefficients $\hat Ta\hat T^{-1}$ multiplying $e^{iE_pt-i\boldsymbol p\cdot\boldsymbol x}$ and $\hat Tb^\dagger\hat T^{-1}$ multiplying $e^{-iE_pt+i\boldsymbol p\cdot\boldsymbol x}$. In $\eta_T\phi(-t,\boldsymbol x)$, replace $\boldsymbol p$ by $-\boldsymbol p$ to obtain precisely these same plane waves. Comparing independent modes proves [time reversal of a complex scalar field](../../../../../time-reversal-of-a-complex-scalar-field.md):

$$
\boxed{\hat Ta(p)\hat T^{-1}=\eta_Ta(p_P),\qquad
\hat Tb^\dagger(p)\hat T^{-1}=\eta_Tb^\dagger(p_P),\quad p_P=(E_p,-\boldsymbol p).}
$$

Taking adjoints gives $\hat Tb(p)\hat T^{-1}=\eta_T^*b(p_P)$. Positive energy is preserved, and an [annihilation operator](../../../../../annihilation-operator.md) remains an [annihilation operator](../../../../../annihilation-operator.md). Time reversal does not exchange particles with [antiparticles](../../../../../antiparticle.md).

The coefficient $\eta_T$ is an [intrinsic time-reversal phase](../../../../../intrinsic-time-reversal-phase.md). Applying $\hat T$ twice gives $\hat T^2a\hat T^{-2}=\eta_T^*\eta_Ta$, so $|\eta_T|=1$; it need not be restricted to $\pm1$. Write $\eta_T=e^{i\vartheta}$ and redefine $a'=e^{i\vartheta/2}a$. Because the phase is conjugated by $\hat T$,

$$
\hat Ta'\hat T^{-1}=e^{-i\vartheta/2}\eta_Ta(p_P)=a'(p_P).
$$

Thus **the scalar intrinsic phase can be absorbed into the annihilation-operator convention**. Redefining $b'=e^{-i\vartheta/2}b$ simultaneously implements the corresponding whole-field rephasing $\phi'=e^{i\vartheta/2}\phi$ and removes the phase from both mode transformations.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
