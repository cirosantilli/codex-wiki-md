<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the [period lattice](../../../../../period-lattice.md) as $\Lambda=\mathbb Z\omega_1+\mathbb Z\omega_2$, with $\omega_1,\omega_2$ real-linearly independent and $\operatorname{Im}(\omega_2/\omega_1)>0$. A [meromorphic function](../../../../../meromorphic-function.md) $f$ is an [elliptic function](../../../../../elliptic-function.md) for this lattice if $f(z+\lambda)=f(z)$ for every $\lambda\in\Lambda$. If it has no [poles](../../../../../pole.md), it is an [entire function](../../../../../entire-function.md) bounded on the closure of a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md). Periodicity makes it bounded on all of $\mathbb C$, so the [Liouville theorem](../../../../../liouville-theorem.md) proves that **an elliptic function without poles is constant**.

Here are the two contour identities needed for counting its zeros and their sum. Choose a positively oriented [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) $P$ whose boundary avoids all zeros and [poles](../../../../../pole.md), and put $h=f'/f$. The [argument principle](../../../../../argument-principle.md) gives

$$
N-P_f=\frac1{2\pi i}\int_{\partial P}h(z)\,dz=0,
$$

because $h$ is periodic and opposite edges cancel. Here $N,P_f$ count zeros and [poles](../../../../../pole.md) with multiplicity. For the weighted integral, let $J_i$ be the integral of $h$ along the edge from a vertex $c$ to $c+\omega_i$. Translating the opposite edges gives

$$
\frac1{2\pi i}\int_{\partial P}z h(z)\,dz
=\frac{\omega_1J_2-\omega_2J_1}{2\pi i}.
$$

The endpoint values of $f$ agree along either edge. A continuous logarithm along the edge therefore changes by $2\pi i n_i$, with $n_i\in\mathbb Z$, and $J_i=2\pi i n_i$. On the other hand, the [residue theorem](../../../../../residue-theorem.md) evaluates the left side as the sum of the zero positions minus the sum of the pole positions, both with multiplicity. Thus the [elliptic divisor-sum identity](../../../../../elliptic-divisor-sum-identity.md) is

$$
\sum_j r_jz_j-\sum_l m_lp_l=\omega_1n_2-\omega_2n_1\in\Lambda.
$$

Under the stated pole hypothesis there is just one pole class, represented by zero, of order $m$. Consequently

$$
\boxed{N=m,\qquad\sum_j r_jz_j\equiv0\pmod\Lambda.}
$$

Changing representatives of the zero classes changes their weighted sum by an element of $\Lambda$, so the congruence is well defined.

The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) is

$$
\wp_\Lambda(z)=\frac1{z^2}+\sum_{0\ne\omega\in\Lambda}
\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

On a bounded set of $z$, the summand is $O(|\omega|^{-3})$ for large $|\omega|$. The lattice sum of $|\omega|^{-3}$ converges in real dimension two, proving [Normal convergence of the Weierstrass elliptic-function series](../../../../../normal-convergence-of-the-weierstrass-elliptic-function-series.md) on compact sets away from $\Lambda$. Hence $\wp$ is a [holomorphic function](../../../../../holomorphic-function.md) there, and at zero its principal part is $z^{-2}$, so it has a double pole. Replacing $\omega$ by $-\omega$ shows that $\wp$ is even. Differentiating the normally convergent series gives

$$
\wp'(z)=-2\sum_{\omega\in\Lambda}(z-\omega)^{-3},
$$

whose absolute convergence permits reindexing by any $\lambda\in\Lambda$. Thus $\wp'$ is periodic and $\wp(z+\lambda)-\wp(z)$ is constant. Substituting $-z-\lambda$ for $z$ and using evenness changes that constant to its negative, so it is zero. This proves that $\wp$ is an [elliptic function](../../../../../elliptic-function.md), with double [poles](../../../../../pole.md) precisely at the lattice points.

The preceding zero count applied to $\wp-a$ says that it has exactly two zeros modulo $\Lambda$, counted with multiplicity. Evenness pairs any zero $z$ with $-z$. If these are distinct classes they must both be simple. If they coincide, $2z\in\Lambda$, and locally $\wp(z+t)=\wp(z-t)$: the zero has even order, which the total count forces to be two. In particular such a zero cannot be a lattice point, where $\wp$ has a pole. **Every finite fibre of the Weierstrass function consists of two opposite simple points or one double nonzero half-period point.**

To obtain the rational representation, first consider an even [elliptic function](../../../../../elliptic-function.md) $g$. The preceding description proves that $\wp:\mathbb C/\Lambda\to\mathbb P^1$ has exactly the fibres $\{z,-z\}$, so $g$ defines a function $A$ of $w=\wp(z)$. Away from the branch values a local inverse of $\wp$ makes $A$ [meromorphic](../../../../../meromorphic-function.md). At a half-period $z_0$, the local expansion is $w-w_0=c t^2+O(t^4)$, with $c\ne0$ because the zero has order exactly two. The Laurent series of $g(z_0+t)$ contains only even powers, and $t^2$ is a holomorphic local coordinate as a function of $w-w_0$. Thus $A$ is [meromorphic](../../../../../meromorphic-function.md) at that value too. At zero the same argument uses $1/w=t^2+O(t^6)$, proving meromorphy at infinity. A [meromorphic function](../../../../../meromorphic-function.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is a [rational function](../../../../../rational-function.md): subtract its finitely many principal parts and use compactness to make the remainder constant. This proves that [even elliptic functions are rational in the Weierstrass function](../../../../../even-elliptic-functions-are-rational-in-the-weierstrass-function.md).

For an arbitrary [elliptic function](../../../../../elliptic-function.md), split $f=f_++f_-$, where $f_\pm(z)=(f(z)\pm f(-z))/2$. The even part is $A(\wp)$. Since $\wp'$ is odd and not identically zero, $f_-/\wp'$ is an even [meromorphic](../../../../../meromorphic-function.md) [elliptic function](../../../../../elliptic-function.md), including at the zeros of $\wp'$ where the quotient may have [poles](../../../../../pole.md). It is therefore $B(\wp)$ for a [rational function](../../../../../rational-function.md) $B$. The [elliptic function-field decomposition](../../../../../elliptic-function-field-decomposition.md) is

$$
\boxed{f(z)=A(\wp(z))+B(\wp(z))\wp'(z),\qquad A,B\in\mathbb C(w).}
$$

The representation is unique: its even and odd parts determine $A$ and $B$, and $\wp$ takes every value on the [Riemann sphere](../../../../../riemann-sphere.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 126](../../paper-126-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
