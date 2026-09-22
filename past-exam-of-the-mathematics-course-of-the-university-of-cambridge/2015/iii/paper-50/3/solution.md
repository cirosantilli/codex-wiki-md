<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret the paired indices $(i,k)$ as incoming and $(j,l)$ as outgoing. For self-conjugate particles in the real [vector representation](../../../../../vector-representation.md) of the [orthogonal group](../../../../../orthogonal-group.md), crossing the second incoming particle with the second outgoing one gives

$$
S_{ik,jl}(\theta)=S_{il,jk}(i\pi-\theta).
$$

The continuation $\theta\mapsto i\pi-\theta$ exchanges the trace and permutation tensor structures and leaves the identity structure fixed. Therefore [crossing symmetry](../../../../../crossing-symmetry.md) imposes

$$
\boxed{S_1(\theta)=S_3(i\pi-\theta),\quad S_2(\theta)=S_2(i\pi-\theta),\quad S_3(\theta)=S_1(i\pi-\theta).}
$$

These are analytic relations; they do not determine the three functions completely.

For [unitarity](../../../../../unitary-operator.md), act on the two-species [tensor product](../../../../../tensor-product.md) with the [O(N)-invariant S-matrix](../../../../../o-n-invariant-s-matrix.md) $S=S_2I+S_3P+S_1K$. The invariant operators obey $P^2=I$, $PK=KP=K$ and $K^2=NK$. Writing $S_a^-=S_a(-\theta)$ and multiplying $S(\theta)S(-\theta)=I$ gives

$$
\boxed{\begin{aligned}
S_2S_2^-+S_3S_3^-&=1,\\
S_2S_3^-+S_3S_2^-&=0,\\
NS_1S_1^-+S_1(S_2^-+S_3^-)+(S_2+S_3)S_1^-&=0.
\end{aligned}}
$$

The three invariant operators are independent for $N\ge2$. Equivalently, the [orthogonal-invariant scattering channels](../../../../../orthogonal-invariant-scattering-channels.md) have amplitudes

$$
s_0=NS_1+S_2+S_3,\qquad s_+=S_2+S_3,\qquad s_-=S_2-S_3,
$$

and each satisfies $s_a(\theta)s_a(-\theta)=1$. The trace singlet, symmetric traceless and antisymmetric channels have dimensions $1$, $N(N+1)/2-1$ and $N(N-1)/2$. For $N=2$ these are $1,2,1$. With [Hermitian analyticity of a two-particle S-matrix](../../../../../hermitian-analyticity-of-a-two-particle-s-matrix.md), $S_a(-\theta)=S_a(\theta)^*$ on the real axis, so each channel has unit modulus. This expresses conservation of scattering probability.

The [Faddeev-Zamolodchikov algebra](../../../../../faddeev-zamolodchikov-algebra.md) orders particle operators by [rapidity](../../../../../rapidity.md). Its [associativity](../../../../../associative-property.md) requires that a product of three operators be independent of parentheses and, in particular, that both sequences of adjacent exchanges give the same final ordered species word with the same coefficient. This is the [Faddeev-Zamolodchikov associativity constraint](../../../../../faddeev-zamolodchikov-associativity-constraint.md), or spectral [Yang-Baxter equation](../../../../../yang-baxter-equation.md). The exchanges do not use the ordinary creation/annihilation [normal ordering](../../../../../normal-ordering.md) convention.

Take $\theta_1>\theta_2>\theta_3$, with $\theta=\theta_1-\theta_2$, $\theta'=\theta_2-\theta_3$, and abbreviate

$$
a_r=S_r(\theta),\qquad b_r=S_r(\theta+\theta'),\qquad c_r=S_r(\theta').
$$

For $N=2$, start with $A_1(\theta_1)A_1(\theta_2)A_2(\theta_3)$ and compare the coefficient of $A_1(\theta_3)A_2(\theta_2)A_1(\theta_1)$. First exchange positions $1,2$, then $2,3$, then $1,2$. The initial equal-index exchange gives

$$
A_1(\theta_1)A_1(\theta_2)=(a_1+a_2+a_3)A_1(\theta_2)A_1(\theta_1)+a_1A_2(\theta_2)A_2(\theta_1).
$$

From the first term, the specified final word is reached through $b_2c_3$; from the second term, the intermediate equal-index exchange uses $b_1$ to produce species $1$, followed by $c_2$. Thus this exchange route has coefficient

$$
C_{121}=(a_1+a_2+a_3)b_2c_3+a_1b_1c_2.
$$

For the other route, first exchange positions $2,3$, then $1,2$, then $2,3$. The first exchange is between different indices and gives $c_2A_1(\theta_1)A_2(\theta_3)A_1(\theta_2)+c_3A_1(\theta_1)A_1(\theta_3)A_2(\theta_2)$. The first term reaches the target through $b_3a_3$, and the second reaches it through $(b_1+b_2+b_3)a_2$. Therefore

$$
C_{212}=a_3b_3c_2+a_2(b_1+b_2+b_3)c_3.
$$

Equate these two coefficients, cancel the common term $a_2b_2c_3$, and rearrange:

$$
\boxed{a_2b_1c_3+a_2b_3c_3+a_3b_3c_2=a_3b_2c_3+a_1b_2c_3+a_1b_1c_2.}
$$

Restoring the three arguments gives the required scalar [Yang-Baxter equation](../../../../../yang-baxter-equation.md). The derivation starts in the ordered physical region $\theta,\theta'>0$; the identity extends to other values by the same scattering [analytic continuation](../../../../../analytic-continuation.md), wherever its factors are defined. **Associativity must hold coefficient by coefficient for every species word; this displayed relation is one necessary component.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
