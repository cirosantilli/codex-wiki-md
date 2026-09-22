<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix [fundamental units](../../../../../fundamental-unit-number-theory.md) $\varepsilon_1,\ldots,\varepsilon_r$ and write $x=\zeta\prod\varepsilon_i^{b_i}$. Rank zero already gives a finite [unit group](../../../../../unit-group.md). Otherwise put $B=\max(1,|b_i|)$. The logarithmic embedding in Dirichlet's theorem has a weighted sum-zero image and is injective on the free exponent lattice. Norm equivalence and that sum-zero condition give an archimedean embedding $\sigma$ with

$$
|\sigma(x)|\le C e^{-cB}.
$$

This is the [small archimedean value of a large unit](../../../../../small-archimedean-value-of-a-large-unit.md). From the equation, $\sigma(\beta y)=1-\sigma(\alpha x)$ is exponentially close to one. Also $h(y)\le h(x)+O(1)$ by the [arithmetic height](../../../../../height-function.md) inequalities for $y=(1-\alpha x)/\beta$, so the fundamental-unit exponents of $y$ have size $O(B)$.

For large $B$, take the small-branch logarithm of $\sigma(\beta y)$. With $y=\eta\prod\varepsilon_i^{c_i}$ it is the nonzero form

$$
\Lambda=\log\sigma(\beta\eta)+\sum_i c_i\log\sigma(\varepsilon_i)-2k\log(-1),\qquad |k|=O(B),
$$

using fixed logarithms and $\log(-1)=\pi i$. The [integer](../../../../../integer.md) $k$ corrects the branch, and nonzero follows since $\beta y=1$ would force $\alpha x=0$. Its upper bound is $|\Lambda|\le C'e^{-cB}$. The assumed effective logarithmic-form estimate for the fixed [algebraic numbers](../../../../../algebraic-number.md) gives $\log|\Lambda|\ge-C''\log(2B)$. Thus $cB\le C''\log(2B)+O(1)$, effectively bounding $B$. The finitely many embeddings and torsion choices give uniform constants. Therefore **there are only finitely many [unit](../../../../../unit-in-a-ring.md) solutions, and their exponents are effectively bounded**.

For the Thue application, take an irreducible integral [binary form](../../../../../binary-form.md) $F$ of degree $d\ge3$ and $m\ne0$. In a [splitting field](../../../../../splitting-field.md), write $F(X,Y)=a\prod_i(X-\rho_iY)$ and put $\theta_i=a\rho_i$, which are [algebraic integers](../../../../../algebraic-integer.md). The integral factors $L_i=aX-\theta_iY$ satisfy $\prod_iL_i=a^{d-1}m$. Each [ideal](../../../../../ideal.md) $(L_i)$ therefore divides one fixed [ideal](../../../../../ideal.md), giving finitely many possibilities. Choose a generator $\delta_i$ for each principal possibility, so $L_i=\delta_i u_i$ with [units](../../../../../unit-in-a-ring.md) $u_i$.

For three distinct roots,

$$
(\theta_2-\theta_3)L_1+(\theta_3-\theta_1)L_2+(\theta_1-\theta_2)L_3=0.
$$

Division by the third term gives a fixed-coefficient [unit](../../../../../unit-in-a-ring.md) equation in $u_1/u_3,u_2/u_3$. Its solutions are finite, hence there are finitely many values of $L_1/L_2$. This ratio determines the rational direction $X:Y$, since the roots are distinct. In a fixed direction, homogeneity and $F(X,Y)=m\ne0$ leave only finitely many [integer](../../../../../integer.md) scales. This proves [Thue theorem](../../../../../thue-theorem.md), and the argument also works for a form with at least three distinct projective roots even if reducible.

The hyperelliptic alternative uses a related factorization for the usual nondegenerate case with squarefree $f$ of degree at least three. For $y^2=f(x)$, [ideals](../../../../../ideal.md) of two different root factors can share primes only above the fixed root differences and the leading coefficient. At other primes their valuations are even. Finite exceptional-prime and ideal-class choices, together with [units](../../../../../unit-in-a-ring.md) modulo squares, reduce the factors to finitely many expressions $\delta_i z_i^2$. Relations between distinct root factors then give simultaneous norm or Pell-type equations. Writing their solutions in [fundamental units](../../../../../fundamental-unit-number-theory.md) and applying the same small-value/logarithmic-form estimates bounds the [unit](../../../../../unit-in-a-ring.md) exponents, hence $x,y$. The common-factor and square-class reductions are essential; a single quadratic norm equation alone can have infinitely many Pell solutions. This outlines the effective hyperelliptic treatment as well as the explicit Thue reduction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
