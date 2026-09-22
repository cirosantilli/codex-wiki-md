<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mathbb H$ be the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) and put $q=e^{2\pi i\tau}$. A weight-$k$ [modular form](../../../../../modular-form.md) for the [modular group](../../../../../modular-group.md) is a holomorphic function on $\mathbb H$ satisfying

$$
f\!\left(\frac{a\tau+b}{c\tau+d}\right)=(c\tau+d)^kf(\tau)\qquad\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SL_2(\mathbb Z),
$$

whose [Fourier expansion](../../../../../fourier-series-split.md) at the [modular cusp](../../../../../cusp-of-a-modular-group.md) at infinity has only nonnegative powers of $q$. These functions form the [vector space](../../../../../vector-space-split.md) $M_k$. Its subspace $S_k$ consists of the [cusp forms](../../../../../cusp-form.md), whose constant [Fourier coefficient](../../../../../fourier-coefficient.md) is zero. For the full [modular group](../../../../../modular-group.md) every cusp is equivalent to infinity, so this is the complete cusp condition. The [matrix](../../../../../matrix.md) $-I$ gives $M_k=0$ for odd $k$, and the [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) excludes nonzero forms of negative weight.

The normalized [Eisenstein series](../../../../../eisenstein-series.md) start as $E_4=1+240q+O(q^2)$ and $E_6=1-504q+O(q^2)$. Consequently the [modular discriminant](../../../../../modular-discriminant.md)

$$
\Delta=\frac{E_4^3-E_6^2}{1728}=q+O(q^2)
$$

is a nonzero [cusp form](../../../../../cusp-form.md) of weight twelve, with order one at infinity. Its contribution there already exhausts the valence formula, so it has no zero in $\mathbb H$. Multiplication by $\Delta$ takes $M_k$ injectively into $S_{k+12}$. Conversely, dividing any member of $S_{k+12}$ by $\Delta$ is holomorphic in $\mathbb H$, has weight $k$, and has no negative power at infinity because its numerator vanishes there. Thus [multiplication by the modular discriminant](../../../../../multiplication-by-the-modular-discriminant.md) gives

$$
\boxed{M_k\xrightarrow{\;f\mapsto\Delta f\;}S_{k+12}\text{ an isomorphism}.}
$$

The [valence formula for the modular group](../../../../../valence-formula-for-the-modular-group.md) shows that a weight-zero form minus its constant term must vanish: otherwise it would be a [cusp form](../../../../../cusp-form.md) with positive order at infinity and total zero order zero. Hence $\dim M_0=1$. A weight-two form satisfies $f(i)=i^2f(i)=-f(i)$, so any nonzero one would contribute at least $1/2$ to the valence formula, exceeding $2/12$. Therefore $M_2=0$.

Every even integer $k\geq4$ has a representation $k=4a+6b$ with $a,b\geq0$. Indeed, if $k/2$ is even, take $b=0$; if it is odd, take $b=1$ and $a=(k-6)/4$. The form $R_k=E_4^aE_6^b$ has constant term one. Taking the constant [Fourier coefficient](../../../../../fourier-coefficient.md) therefore maps $M_k$ onto $\mathbb C$, with kernel $S_k=\Delta M_{k-12}$. Starting with the negative-weight vanishing and the two initial dimensions gives

$$
\dim M_k=1+\dim M_{k-12}\quad(k\geq4\text{ even}),
$$

and hence the [dimension of level-one modular forms](../../../../../dimension-of-level-one-modular-forms.md) is

$$
\boxed{\dim M_k=\begin{cases}\lfloor k/12\rfloor,&k\equiv2\pmod{12},\\\lfloor k/12\rfloor+1,&k\not\equiv2\pmod{12},\end{cases}\qquad k\geq0\text{ even}.}
$$

This also proves finite dimensionality, rather than presupposing it in the recurrence.

For the generation assertion, if $f\in M_k$ has constant coefficient $a_0$, subtract $a_0R_k$. The difference is a [cusp form](../../../../../cusp-form.md), and so equals $\Delta h$ with $h\in M_{k-12}$. Induction on weight expresses $h$ as a polynomial in $E_4,E_6$; substituting the polynomial expression for $\Delta$ does the same for $f$. Constants start the induction, while weight two contributes nothing. The result is a weighted homogeneous polynomial, assigning weights four and six to its variables. In fact the monomials $E_4^aE_6^b$ with $4a+6b=k$ number exactly the displayed dimension: $b$ runs from zero to $\lfloor k/6\rfloor$ with parity $k/2$. Their spanning property therefore makes them a basis in each weight. This identifies the [polynomial ring of level-one modular forms](../../../../../polynomial-ring-of-level-one-modular-forms.md):

$$
\boxed{M_*(SL_2(\mathbb Z))=\mathbb C[E_4,E_6].}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
