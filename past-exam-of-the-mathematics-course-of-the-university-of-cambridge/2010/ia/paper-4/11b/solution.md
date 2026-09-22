<h1 id="11b/solution">Solution</h1>

↑ **Parent:** [11B](../11b.md)

Work in an [inertial frame](../../../../../inertial-frame.md), take all masses to be constant, and assume the internal forces obey the pairwise relation from [Newton's third law](../../../../../newton-s-third-law.md) $F_{ij}=-F_{ji}$. For the [angular momentum](../../../../../angular-momentum.md) result, also assume these pair forces are central, so $F_{ij}$ is parallel to $r_i-r_j$ and its pair torque vanishes. The equations from [Newton's second law](../../../../../newton-s-second-law.md) are

$$
m_i\ddot r_i=F_i+\sum_{j\ne i}F_{ij}.
$$

Summing them and pairing the internal forces gives

$$
\boxed{\frac{dP}{dt}=F,\qquad
P=\sum_i m_i\dot r_i,\qquad F=\sum_iF_i.}
$$

About a fixed point $a$, define the total [angular momentum](../../../../../angular-momentum.md) and external [torque](../../../../../torque.md) by

$$
L_a=\sum_i(r_i-a)\times m_i\dot r_i,\qquad
G_a=\sum_i(r_i-a)\times F_i.
$$

Differentiation produces no velocity term because $\dot r_i\times m_i\dot r_i=0$. Grouping internal terms into pairs gives

$$
\frac{dL_a}{dt}
=G_a+\sum_{i<j}\bigl[(r_i-a)\times F_{ij}+(r_j-a)\times F_{ji}\bigr]
=G_a+\sum_{i<j}(r_i-r_j)\times F_{ij}.
$$

Each final [cross product](../../../../../cross-product.md) is zero by centrality, proving $\boxed{dL_a/dt=G_a}$. Equal and opposite internal forces give [momentum conservation](../../../../../momentum-conservation.md) when the total external force is zero, but do not in general make their internal [torques](../../../../../torque.md) cancel; the central-force assumption supplies that extra step.

Let $M=\sum_i m_i$ and let the [centre of mass](../../../../../center-of-mass.md) be $R=M^{-1}\sum_i m_i r_i$, so $P=M\dot R$. For an arbitrary moving reference point $a(t)$, the same differentiation gives

$$
\frac{dL_{a(t)}}{dt}=G_{a(t)}-\dot a\times P.
$$

Taking $a=R$, the extra term is $-\dot R\times M\dot R=0$. Therefore the corresponding [angular momentum about the centre of mass](../../../../../angular-momentum-about-the-centre-of-mass.md) satisfies

$$
\boxed{\frac{dL_R}{dt}=G_R.}
$$

Its definition using velocities relative to $\dot R$ agrees with the one above, since $\sum_i m_i(r_i-R)=0$ makes $\sum_i(r_i-R)\times m_i\dot R=0$. Thus this result remains true even when the [centre of mass](../../../../../center-of-mass.md) accelerates.

Finally take the common mass to be $m$ and $F_i=-k\dot r_i$, with constant $k$. About either a fixed point or the [centre of mass](../../../../../center-of-mass.md),

$$
G=-k\sum_i(r_i-a)\times\dot r_i=-\frac km L.
$$

The angular-momentum equation becomes $\dot L=-(k/m)L$. Multiplying by the integrating factor $e^{kt/m}$ gives $\frac{d}{dt}(e^{kt/m}L)=0$, hence the [angular momentum decay under uniform linear drag](../../../../../angular-momentum-decay-under-uniform-linear-drag.md) is

$$
\boxed{L(t)=L(0)e^{-kt/m}.}
$$

The common mass and common drag coefficient ensure that the same decay factor applies to every term.

## ↑ Ancestors (10)

1. [11B](../11b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
