# Spanning Proof for Partial Sum Vectors via Change-of-Basis Matrix

## Goal

We are given that $\mathcal{B}_v = \{v_1, \ldots, v_n\}$ is a basis for a vector space $V$. We define a new set of vectors $\mathcal{B}_u = \{u_1, \ldots, u_n\}$ where $u_k = \sum_{i=1}^k v_i$. We want to prove that $\mathcal{B}_u$ also **spans** $V$.

## Definition of Spanning

To show $\mathcal{B}_u$ spans $V$, we must show that for *any* arbitrary vector $w \in V$, there exist scalars $d_1, \ldots, d_n$ such that:
$$w = d_1 u_1 + d_2 u_2 + \cdots + d_n u_n$$
This is equivalent to showing that any vector $w$ has a coordinate representation with respect to the basis $\mathcal{B}_u$.

## Using Coordinates and Change of Basis

Let $[w]_v$ denote the coordinate vector of $w$ with respect to the basis $\mathcal{B}_v$, and $[w]_u$ denote the coordinate vector of $w$ with respect to the (potential) basis $\mathcal{B}_u$.
$$[w]_v = \begin{pmatrix} c_1 \\ \vdots \\ c_n \end{pmatrix} \quad \text{such that } w = \sum_{i=1}^n c_i v_i$$
$$[w]_u = \begin{pmatrix} d_1 \\ \vdots \\ d_n \end{pmatrix} \quad \text{such that } w = \sum_{k=1}^n d_k u_k$$

We can relate these coordinate systems using a **change-of-basis matrix**. Let $P$ be the matrix whose columns are the coordinate vectors of the $u_k$'s expressed in terms of the $v_j$'s.

* $u_1 = 1v_1 + 0v_2 + \dots + 0v_n \implies [u_1]_v = \begin{pmatrix} 1 \\ 0 \\ \vdots \\ 0 \end{pmatrix}$
* $u_2 = 1v_1 + 1v_2 + \dots + 0v_n \implies [u_2]_v = \begin{pmatrix} 1 \\ 1 \\ \vdots \\ 0 \end{pmatrix}$
* $\vdots$
* $u_n = 1v_1 + 1v_2 + \dots + 1v_n \implies [u_n]_v = \begin{pmatrix} 1 \\ 1 \\ \vdots \\ 1 \end{pmatrix}$

Thus, the change-of-basis matrix from $\mathcal{B}_u$ to $\mathcal{B}_v$ is:
$$P = \begin{pmatrix} [u_1]_v & [u_2]_v & \cdots & [u_n]_v \end{pmatrix} = \begin{pmatrix}
1 & 1 & 1 & \cdots & 1 \\
0 & 1 & 1 & \cdots & 1 \\
0 & 0 & 1 & \cdots & 1 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \cdots & 1
\end{pmatrix}$$
This matrix $P$ transforms $u$-coordinates to $v$-coordinates:
$$[w]_v = P [w]_u$$

## Invertibility is Key

The matrix $P$ is an $n \times n$ upper triangular matrix with all diagonal entries equal to 1.
* Its determinant is $\det(P) = 1^n = 1 \neq 0$.
* Alternatively, it clearly has $n$ pivots (one on the diagonal of each column).
Therefore, $P$ is **invertible**, and its inverse $P^{-1}$ exists.

## The Argument for Spanning

1.  Start with the coordinate transformation rule: $[w]_v = P [w]_u$.
2.  Since $P$ is invertible, multiply by $P^{-1}$ on the left:
    $$P^{-1} [w]_v = P^{-1} P [w]_u = I [w]_u = [w]_u$$
    So, we have the reverse transformation:
    $$[w]_u = P^{-1} [w]_v$$
3.  Now, consider any arbitrary vector $w \in V$.
4.  Because $\mathcal{B}_v = \{v_1, \ldots, v_n\}$ is a basis (and thus spans $V$), we know its coordinate vector $[w]_v$ **must exist**.
5.  Since $P^{-1}$ exists, we can **always compute** the coordinate vector $[w]_u$ using the formula $[w]_u = P^{-1} [w]_v$.
6.  The fact that we can *always* find the coordinate vector $[w]_u$ (which contains the coefficients $d_1, \ldots, d_n$) for *any* $w \in V$ means, by definition, that the set $\mathcal{B}_u = \{u_1, \ldots, u_n\}$ **spans** $V$.

In essence, the invertibility of the change-of-basis matrix guarantees that if the original set spans the space, the new set also spans the space, because we can translate representations back and forth uniquely.