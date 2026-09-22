<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [Dedekind factorization theorem](../../../../dedekind-factorization-theorem.md) says: if $K=\mathbb Q(\theta)$ with $\theta$ integral, [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) $f\in\mathbb Z[X]$, and the rational prime $p$ does not divide $[\mathcal O_K:\mathbb Z[\theta]]$, factor $\bar f=\prod_i\bar f_i^{e_i}$ into distinct monic irreducibles over $\mathbb F_p$. Then the distinct [prime ideals](../../../../prime-ideal.md) above $p$ are $P_i=(p,f_i(\theta))$, with [integer](../../../../integer-split.md) lifts $f_i$, and

$$
\boxed{(p)=\prod_iP_i^{e_i},\qquad N(P_i)=p^{\deg\bar f_i}.}
$$

The index condition is part of the theorem and must be checked before applying it at a ramified prime.

For this cubic, $X^3-6$ is Eisenstein and has [discriminant](../../../../discriminant.md) $-972$. We first verify $\mathcal O_K=\mathbb Z[\theta]$. The square of the index divides 972, so only two and three can divide the index. If either prime $p$ divided it, the finite quotient [group](../../../../group-split.md) would contain an element of order $p$, giving an integral element $(a+b\theta+c\theta^2)/p$ with digits $0\le a,b,c<p$, not all zero. Its [field norm](../../../../field-norm.md) is

$$
\frac{a^3+6b^3+36c^3-18abc}{p^3}.
$$

For $p=2$, the numerator has valuation zero if $a=1$, valuation one if $a=0,b=1$, and valuation two if $a=b=0,c=1$. For $p=3$ the same three cases, according to the first nonzero digit, give valuations zero, one and two. None gives an [integer](../../../../integer-split.md) [field norm](../../../../field-norm.md) after dividing by $p^3$, contradicting integrality. Thus the index is one.

Multiplication by $a+b\theta$ in the [power basis](../../../../power-basis.md), or the product over the three conjugates, gives $\boxed{N(a+b\theta)=a^3+6b^3}$. Define

$$
\begin{aligned}
P_2&=(2,\theta),&P_3&=(3,\theta),\\
P_5&=(5,\theta-1),&Q_5&=(5,\theta^2+\theta+1),\\
P_{7,r}&=(7,\theta-r)&& (r=3,5,6).
\end{aligned}
$$

Reduction of the cubic gives $X^3$ at two and three, $(X-1)(X^2+X+1)$ at five, and $(X-3)(X-5)(X-6)$ at seven. The quadratic factor at five is irreducible since its [discriminant](../../../../discriminant.md) is two, a nonsquare modulo five. Hence

$$
\boxed{(2)=P_2^3,\quad(3)=P_3^3,\quad(5)=P_5Q_5,\quad(7)=P_{7,3}P_{7,5}P_{7,6}.}
$$

The [norms](../../../../norm.md) are respectively $2,3,5,25,7,7,7$. [Norms](../../../../norm.md) and reduction of the elements at those primes give

$$
\boxed{\begin{aligned}
(\theta)&=P_2P_3,&(\theta-1)&=P_5,&(\theta-2)&=P_2,\\
(\theta-3)&=P_3P_{7,3},& (\theta+4)&=P_2P_5P_{7,3}.
\end{aligned}}
$$

For example their absolute element [field norms](../../../../field-norm.md) are $6,5,2,21,70$; each indicated prime divides the element by substitution in its [residue field](../../../../residue-field.md), and the product of the indicated [ideal norms](../../../../ideal-norm.md) already equals that absolute [field norm](../../../../field-norm.md). Thus no additional factor or exponent is possible.

In the [ideal](../../../../ideal.md) of the specified quotient every prime exponent cancels:

$$
(\mu)=\frac{P_2^2(P_3P_{7,3})P_5}{(P_2P_3)(P_2P_5P_{7,3})}=\mathcal O_K.
$$

Equality with the [unit ideal](../../../../unit-ideal.md) implies that both $\mu$ and its inverse are integral, so $\boxed{\mu\text{ is a unit}}$. For the real root, $1<\theta<2$. The numerator is negative and has absolute value less than two, while the denominator is greater than five. Thus $-2/5<\mu<0$, proving $\boxed{\mu\ne\pm1}$. Its [field norm](../../../../field-norm.md) is $-1$, consistent with the [ideal](../../../../ideal.md) calculation.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
