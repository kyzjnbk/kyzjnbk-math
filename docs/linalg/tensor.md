# Tensor

## Calculation

### Kronecker product


If $A$ is an $m \times n$ matrix and $B$ is a $p \times q$ matrix, then the Kronecker product $A \otimes B$ is the $pm \times qn$ block matrix:

![](tensor.asserts/kronecker_prod_1.svg)

more explicitly:

![](tensor.asserts/kronecker_prod_2.svg)

!!! example
    
    ![](tensor.asserts/kronecker_prod_example_1.svg)

vector case (row or column form):

\begin{align}
a\otimes b
&=
(\begin{array}{ccc} a_1 & \dots & a_n \end{array})
\otimes
(\begin{array}{ccc} b_1 & \dots & b_m \end{array}) \\
&=
(\begin{array}{ccccccc} a_1 b_1 & \dots & a_1 b_m & \dots & a_n b_1 & \dots & a_n b_m \end{array})
\end{align}

and

\begin{align}
a\otimes b
&=
(\begin{array}{ccc} a_1 & \dots & a_n \end{array})
\otimes
\left(\begin{array}{c} b_1 \\ \dots \\ b_m \end{array}\right) \\
&=
\left(
    \begin{array}{ccccccc} a_1 b_1 & \dots & a_n b_1 \\ \vdots & \ddots & \vdots \\ a_1 b_m & \dots & a_n b_m \end{array}
\right)
\end{align}

see also:

- [Wikipedia](https://en.wikipedia.org/wiki/Kronecker_product)

### Khatri-Rao product

In mathematics, the Khatri–Rao product is defined as:

![](tensor.asserts/khatri-rao_prod_1.svg)

!!! example

    if A and B both are 2 × 2 partitioned matrices e.g.:

    ![](tensor.asserts/khatri-rao_prod_example_1.svg)

    we obtain:

    ![](tensor.asserts/khatri-rao_prod_example_2.svg)

see also:

- [Wikipedia](https://en.wikipedia.org/wiki/Khatri%E2%80%93Rao_product)

### Hadamard product

**Only for matrices of equal size.**
Also known as the **element-wise product**, **entrywise product**, or Schur product.

$$
(A\odot B)_{ij} = A_{ij} B_{ij}
$$

!!! example
    
    ![](tensor.asserts/hadamard_prod_example_1.svg)

### n-mode tensor-matrix product

The n-mode (matrix) product of a tensor $\mathcal A \in \mathbb{R}^{I_1 \times I_2 \times \ldots \times I_N}$
with a matrix $\mathbf U \in \mathbb{R}^{J \times I_n}$ is denoted by $\mathcal{A} \times_n \mathbf U$
and is of size $I_1 \times \ldots I_{n-1} \times J \times I_{n+1} \times \ldots \times N$.
Elementwise, we have

$$\left(\mathcal A \times_n \mathbf U \right)_{i_1\ldots i_{n-1}\ j\ i_{n+1} \ \ldots \ i_N} = \sum_{i_n=1}^{I_n} a_{i_1i_2\ldots i_N }\ u_{j i_n}.$$

For multiple n-mode product the order is irrelevant:

$$
\text{for } n\neq m: A \times_m U \times_n V = A \times_n V \times_m U
$$

For multiple n-mode product with the same n the order is relevant:

$$
A \times_n U \times_n V = A \times_n (VU)
$$
