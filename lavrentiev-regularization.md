# Lavrentiev regularization

↑ **Parent:** [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)

For a positive self-adjoint [linear operator](linear-operator.md) $A$, Lavrentiev regularization shifts $A$ itself rather than $A^*A$. In a finite-dimensional positive-definite problem, writing $y^\delta=Ax+e$ gives error coefficients $(e_i-\alpha x_i)/(\lambda_i+\alpha)$ in its [orthonormal eigenbasis](orthonormal-eigenbasis.md). Consequently $\|x_\alpha^\delta-x\|\leq\delta/(\lambda_1+\alpha)+\alpha\|x\|/(\lambda_1+\alpha)\leq\delta/\alpha+\alpha\|x\|/\lambda_1$. A known bound $X\geq\|x\|$ permits $\alpha=\sqrt{\delta\lambda_1/X}$, giving a robust bound $2\sqrt{\delta X/\lambda_1}$. For fixed positive $\lambda_1$, the sharper finite-dimensional estimate can give a linear noise rate with a smaller parameter; regularization is then a conditioning choice, not a cure for nonexistence of the inverse.

## ↑ Ancestors (6)

1. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
2. [Inverse problem](inverse-problem-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/5/c/solution.md)
