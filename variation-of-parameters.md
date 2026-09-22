# Variation of parameters

↑ **Parent:** [Second-order linear differential equation](second-order-linear-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variation_of_parameters)

Variation of parameters replaces the constants in a complementary solution by functions to construct a particular solution.

For the [inhomogeneous linear differential equation](inhomogeneous-linear-differential-equation.md) $y''+py'+qy=r$, assume $p,q,r$ are [continuous functions](continuous-function.md) on an [interval](interval-mathematics.md) $I$, and $y_1,y_2$ are [linearly independent](linear-independence.md) [homogeneous solutions](homogeneous-solution.md) there. With $W=W(y_1,y_2)$ and $x_0\in I$, [variation of parameters](variation-of-parameters.md) constructs the [particular solution](particular-solution.md)

$$
y_p(x)=-y_1(x)\int_{x_0}^x\frac{y_2(s)r(s)}{W(s)}\,ds+y_2(x)\int_{x_0}^x\frac{y_1(s)r(s)}{W(s)}\,ds.
$$

The [Wronskian](wronskian.md) has no zeros on $I$, so these quotients are defined. For $Ay''+By'+Cy=F$, normalize first: $r=F/A$, not $F$.[NIST Digital Library of Mathematical Functions; §1.13(iii), equations 1.13.8–1.13.10: normalized inhomogeneous equation and variation-of-parameters formula](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

To derive the formula, write $y_p=u_1y_1+u_2y_2$ and impose $u_1'y_1+u_2'y_2=0$. This auxiliary choice removes extra terms from the first [derivative](derivative.md). Substitution into the [inhomogeneous linear differential equation](inhomogeneous-linear-differential-equation.md) leaves $u_1'y_1'+u_2'y_2'=r$. The two [linear equations](linear-equation.md) for $u_1',u_2'$ have [determinant](determinant.md) $W$, and [Cramer's rule](cramer-s-rule.md) gives

$$
u_1'=-\frac{y_2r}{W},\qquad u_2'=\frac{y_1r}{W}.
$$

Integrating from $x_0$ makes $y_p(x_0)=y_p'(x_0)=0$. Arbitrary integration constants contribute only [homogeneous solutions](homogeneous-solution.md); adding $c_1y_1+c_2y_2$ supplies the [general solution](general-solution.md).

For a worked example, use the same [homogeneous solutions](homogeneous-solution.md) $e^{-x},e^{2x}$ and the [forcing term](forcing-term.md) $r=6e^{3x}$ in $y''-y'-2y=6e^{3x}$. With $x_0=0$ and $W=3e^x$,

$$
u_1'=-2e^{4x},\qquad u_2'=2e^x,\qquad u_1=-\tfrac12(e^{4x}-1),\qquad u_2=2(e^x-1).
$$

Consequently the [particular solution](particular-solution.md) selected by zero [initial conditions](initial-condition.md) is

$$
y_p(x)=\tfrac32e^{3x}+\tfrac12e^{-x}-2e^{2x}.
$$

Its value and first [derivative](derivative.md) vanish at zero. Direct substitution confirms the [forcing term](forcing-term.md): the [differential operator](differential-operator.md) $L[y]=y''-y'-2y$ annihilates the last two terms and maps $e^{3x}$ to $4e^{3x}$. The two integrals therefore build a response from known [homogeneous solutions](homogeneous-solution.md), even when the [forcing term](forcing-term.md) has no convenient elementary guess.

## ↑ Ancestors (8)

1. [Second-order linear differential equation](second-order-linear-differential-equation.md)
2. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Abel's identity](abel-s-identity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-72/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/3/d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-2/7c/b/solution.md)
- [Radial modified Helmholtz equation](radial-modified-helmholtz-equation.md)
- [Variation of parameters](variation-of-parameters.md)
