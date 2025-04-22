## Rigorous Explanation

**1. Stronger condition ⇒ trivial pairwise intersections**

Suppose for each $k$:
$$
W_k \cap \Bigl(\sum_{j \neq k} W_j\Bigr) = \{0\}.
$$
Then for any fixed $k$ and any $i \neq k$:
$$
W_k \cap W_i 
\;\subset\;
W_k \cap \Bigl(\sum_{j \neq k} W_j\Bigr)
= \{0\},
$$
hence
$$
W_k \cap W_i = \{0\}.
$$

**2. Trivial pairwise intersections ⇏ stronger condition**

Pairwise triviality only asserts
$$
W_i \cap W_j = \{0\},\quad i \neq j,
$$
but does **not** forbid a nonzero vector in, say, $W_3$ from being the sum of vectors in $W_1$ and $W_2$.

### Counterexample in $\mathbb{R}^2$

Let
$$
W_1 = \mathrm{span}\{(1,0)\},\quad
W_2 = \mathrm{span}\{(0,1)\},\quad
W_3 = \mathrm{span}\{(1,1)\}.
$$
Then $W_i \cap W_j = \{0\}$ for all $i \neq j$, yet
$$
W_1 + W_2 = \mathbb{R}^2,
\quad
W_3 \cap (W_1 + W_2) = W_3 \neq \{0\},
$$
so $\sum_i W_i$ fails to be a direct sum despite trivial pairwise intersections.

---

## Intuitive Explanation

- **What pairwise‑checking misses**  
  Checking each pair $W_i, W_j$ is like confirming no single actor perfectly impersonates another—fine, but you could still impersonate “Actor A” by blending snippets of “Actor B” and “Actor C.”  Likewise, even if no vector lies in both $W_1$ and $W_2$, a vector in $W_3$ might “sound” exactly like a bit of $W_1$ plus a bit of $W_2$.

- **Why the stronger test matters**  
  Requiring
  $$
  W_k \cap \Bigl(\sum_{j \neq k} W_j\Bigr) = \{0\}
  $$
  guarantees *no* vector in $W_k$ can be built from *any* combination of the other subspaces.  Equivalently, it enforces the uniqueness of decomposition in a direct sum:
  $$
  w_1 + w_2 + \cdots + w_l = 0
  \quad\Longrightarrow\quad
  w_1 = w_2 = \cdots = w_l = 0.
  $$
  Trivial pairwise intersections alone are too weak to ensure this “no‑mixtures” property.
