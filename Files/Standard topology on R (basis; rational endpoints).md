<br />
<br />

Date Created: 04/02/2022 14:47:46
Tags: #Proposition #Closed 

Proved by: [[Q is dense in R]], [[Criteria for collection to be a basis for an existing topology]]
Generalizations: _Not Applicable_

!!! ad-Proposition Proposition.

_The standard topology_ $\mc{T}\l(<\r)$ _on $\mb{R}$ can be generated by the basis_
$$\begin{equation}
    \mc{B}'\coloneqq\l\{B\in\mc{P}\l(\mb{R}\r)\mid\ex a,b\in\mb{Q}:a<b\land B=\l(a,b\r)\r\}
\end{equation}$$
_containing open intervals with rational endpoints._

--- admonition

_Proof_. First observe that if $\l(a,b\r)\in\mc{B}'$, then $a,b\in\mb{R}$ too. It follows that $\mc{B}'\subseteq\mc{B}\subseteq\mc{T}\l(\mc{B}\r)=\mc{T}\l(<\r)$ where
$$\begin{equation}
    \mc{B}\coloneqq\l\{B\in\mc{P}\l(\mb{R}\r)\mid\ex a,b\in\mb{R}:a<b\land B=\l(a,b\r)\r\}.
\end{equation}$$
Take $U\in\mc{T}\l(<\r)$ and $x\in U$, so, by definition of the topology generated by $\mc{B}$, there exists $\l(a,b\r)\in\mc{B}$ such that $x\in\l(a,b\r)\subseteq U$. Since $\mb{Q}$ is dense in $\mb{R}$, we see that there exist rational numbers $a',b'\in\mb{Q}$ such that
$$\begin{equation}
    a<a'<x\ \ \ \ \textrm{and}\ \ \ \ x<b'<b.
\end{equation}$$
Observe then that $\l(a',b'\r)\in\mc{B}$ and that $x\in\l(a',b'\r)\subseteq\l(a,b\r)\subseteq U$.<span style="float:right;">$\blacksquare$</span>