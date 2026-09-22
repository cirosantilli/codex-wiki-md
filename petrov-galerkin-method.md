# Petrov-Galerkin method

↑ **Parent:** [Galerkin method](galerkin-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Petrov–Galerkin_method)

The [Petrov-Galerkin method](petrov-galerkin-method.md) chooses an approximate solution $u_h$ in a finite-dimensional trial [vector space](vector-space-split.md) $V_h$ and tests a [weak formulation](weak-formulation.md) against a possibly different test space $W_h$. For a [bilinear form](bilinear-form.md) $a$ and a [linear functional](linear-functional.md) $\ell$, it imposes $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in W_h$. Taking $W_h=V_h$ recovers the usual [Galerkin method](galerkin-method.md). Different test functions can alter stability and accuracy; the [Galerkin orthogonality](galerkin-orthogonality.md) is then against the test space and need not be an [orthogonal projection](orthogonal-projection.md) in an [energy norm](energy-norm.md).

## ↑ Ancestors (8)

1. [Galerkin method](galerkin-method.md)
2. [Weak solution](weak-solution.md)
3. [Solution of a partial differential equation](solution-of-a-partial-differential-equation.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Finite element method](finite-element-method.md)
- [Galerkin orthogonality](galerkin-orthogonality.md)
- [Petrov-Galerkin method](petrov-galerkin-method.md)
