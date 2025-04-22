Let $V$ be a finite‑dimensional vector space. We show that any two bases of $V$ have the same number of elements.

---

## Steinitz Exchange Lemma

**Lemma.**  
Let  
- $W = \{w_1, \dots, w_n\}$ be a spanning set of $V$, and  
- $B = \{b_1, \dots, b_m\}$ be a linearly independent set in $V$.  

Then $m \le n$. Moreover, one can successively replace $m$ elements of $W$ by the $b_j$ to obtain a new spanning set  
$$
\{b_1, \dots, b_m\} \;\cup\; T,
$$  
where $T \subseteq W$ has cardinality $n - m$.

### Proof of the Lemma

We construct by induction a sequence of spanning sets  
$$
W_0 \;\longmapsto\; W_1 \;\longmapsto\;\cdots\;\longmapsto\; W_m
$$  
each of size $n$, where at step $k$ we replace one element of $W_{k-1}$ by $b_k$.

1. **Base case ($k = 0$).**  
   Set $W_0 = W$. By hypothesis $|W_0| = n$ and $\mathrm{span}(W_0) = V$.

2. **Inductive step.**  
   Assume $W_{k-1}$ spans $V$ and $|W_{k-1}| = n$. Since $W_{k-1}$ spans,  
   $$
   b_k \;=\; \sum_{w \in W_{k-1}} \alpha_w \, w,
   $$  
   for some scalars $\alpha_w$, and because $\{b_1,\dots,b_{k-1}\}$ is independent, at least one coefficient $\alpha_{w^*}$ is nonzero.

   - **Dropping $w^*$:**  
     Rewrite the above as
     $$
     b_k = \alpha_{w^*}\,w^* \;+\;\sum_{w \neq w^*}\alpha_w\,w.
     $$
     Solve for $w^*$:
     $$
     w^* 
       = \frac{1}{\alpha_{w^*}}\,b_k 
         \;-\;\sum_{w \neq w^*}\frac{\alpha_w}{\alpha_{w^*}}\,w.
     $$
     The right-hand side is a linear combination of $b_k$ and the remaining $w\in W_{k-1}\setminus\{w^*\}$, so
     $$
     w^* \;\in\; \mathrm{span}\bigl(\{b_k\}\;\cup\;(W_{k-1}\setminus\{w^*\})\bigr).
     $$
   - **Conclusion:**  
     Therefore the new set
     $$
     W_k \;=\;\bigl(W_{k-1}\setminus\{w^*\}\bigr)\;\cup\;\{b_k\}
     $$
     still spans $V$, and $|W_k| = n$.

After $m$ replacements we obtain  
$$
W_m = \{b_1, \dots, b_m\} \;\cup\; T,
\quad |T| = n - m.
$$  
Since $\{b_1,\dots,b_m\}$ is independent, we conclude $m \le |W_m| = n$.

$\Box$

---

## Proof of Theorem 7.1

Let  
$$
B = \{b_1, \dots, b_m\}
\quad\text{and}\quad
B' = \{b'_1, \dots, b'_n\}
$$  
be two bases of $V$. Then each of $B$ and $B'$ is both independent and spanning.

1. Applying the Exchange Lemma to the independent set $B$ and the spanning set $B'$ gives  
   $$
   m = |B| \;\le\; |B'| = n.
   $$
2. Swapping roles, applying the Lemma to $B'$ and $B$ gives  
   $$
   n = |B'| \;\le\; |B| = m.
   $$
3. Hence $m \le n$ and $n \le m$, so $m = n$.

Thus all bases of $V$ have the same cardinality, called the **dimension** of $V$.

$\Box$