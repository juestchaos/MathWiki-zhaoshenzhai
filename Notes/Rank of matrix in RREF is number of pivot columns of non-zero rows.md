---
mathLink: Rank of matrix in RREF is $|$pivot columns$|/|$non-zero rows$|$
---

<br />
<br />

Date Created: 07/06/2022 18:06:05
Tags: #Proposition #Closed

Proved by: [Elementary matrices/operations are rank-preserving](Elementary%20matrices%20slash%20operations%20are%20rank-preserving.md), [[Linearly independent subset cannot contain the zero vector]]
Justifications: [[Gaussian Algorithm]]

Generalizations: _Not Applicable_
Counterexamples: _Not Applicable_

``` ad-Proposition
title: Proposition.

_Let $K$ be a field and consider a matrix $A\in\mat{m\times n}{K}$ for some fixed $m,n\in\N^\ast$. Letting $R$ be a reduced row-echelon form of $A$, we can compute $\rank A$ by counting the number of non-zero rows or pivot columns of $R$._

```

_Proof_. Since $R$ is obtained via a finite number of elementary row operations on $A$, which preserve rank, we see that $\rank A=\rank R$.
* (Non-zero rows): Let $r\in\N$ be the number of non-zero rows of $R$. Since $R$ is in reduced row-echelon form, each non-zero row $\v{r}_i$ of $R$ contains a leading 1 in its pivot column $k_i$, so $\l(\v{r}_i\r)_{k_i}=1$ and $\l(\v{r}_l\r)_{k_i}=0$ for all $l\neq i$. Hence these rows are linearly independent, for suppose that there are coefficients $\alpha_1,\dots,\alpha_n\in K$ such that $\sum_{i=1}^r\alpha_i\v{r}_i=\v{0}$. Then, for all $i\in\l\{1,\dots,r\r\}$, its $k_i^\textrm{th}$ component is
$$\begin{equation}
    \l(\sum_{i=1}^r\alpha_i\v{r}_i\r)_{\!k_i}=0,
\end{equation}$$
so $\alpha_i\l(\v{r}_i\r)_{k_i}=\alpha_i\l(1\r)=\alpha_i=0$. Since linearly independent sets must not contain zero vectors, we see that those rows form a maximally independent subset of all the rows of $R$, and hence a basis thereof. The result follows since $\rank R=\dim\row R=r$.

* (Pivot columns): Since every non-zero row corresponds uniquely to its pivot column, we see that the number of non-zero rows coincides with the number of pivot columns. The result follows.<span style="float:right;">$\blacksquare$</span>
