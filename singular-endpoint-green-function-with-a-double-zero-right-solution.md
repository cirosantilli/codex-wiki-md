# Singular-endpoint Green function with a double-zero right solution

↑ **Parent:** [Dirichlet Green function](dirichlet-green-function.md)

For $0<x<1$, consider the [self-adjoint differential operator](self-adjoint-differential-operator.md) $L=(p\,d/dx)'+q$ with $p=e^{-x}/(1-x)$ and $q=-e^{-x}/(1-x)^2$. The homogeneous solutions $u=x$ and $v=e^x-ex$ satisfy the left and right zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md). Their [Wronskian](wronskian.md) is $(x-1)e^x$, and $pW=-1$. Thus the displayed [Dirichlet Green function](dirichlet-green-function.md) is continuous, zero at both endpoints, and has unit flux jump $p(s)[G_x(s^+,s)-G_x(s^-,s)]=1$.

The right solution has a double zero, $v(s)\sim e(1-s)^2/2$. Consequently $G(x,s)F(s)$ is integrable at $s=1$ for fixed interior $x$ when $F(s)=-e^{-s}/(1-s)^2$, even though $F$ itself is not integrable there. The endpoint zero of the [Wronskian](wronskian.md) causes no loss of this construction because the weighted [Wronskian](wronskian.md) $pW$ stays nonzero. This illustrates the need to retain the [integrating factor](integrating-factor.md) when constructing a Green function at a singular endpoint.

## ↑ Ancestors (6)

1. [Dirichlet Green function](dirichlet-green-function.md)
2. [Green's function](green-s-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2014/2/a/solution.md)
