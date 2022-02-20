<br />
<br />

Date Created: 19/02/2022 17:12:33
Tags: #Proposition #Closed 

Proved by: [[Distribution of conjunction over disjunction]]
Generalizations: _Not Applicable_

Examples: _Not Applicable_
Counterexamples: _Not Applicable_

``` ad-Proposition
title: Proposition.

_Let $v$ be a set and fix a subset $u\subseteq V$. Then $v\comp\l(v\comp u\r)=u$._

```

_Proof_. Take $x\in v\comp\l(v\comp u\r)$. The result follows from the following chain of equivalences:
$$\begin{alignat}{2}
    x\in v\comp\l(v\comp u\r)&\Leftrightarrow x\in v\land x\not\in v\comp u&&\textrm{Definition of relative complement}\\
    &\Leftrightarrow x\in v\land\lnot\l(x\in v\comp u\r)&&\textrm{Definition of }\not\in\\
    &\Leftrightarrow x\in v\land\lnot\l(x\in v\land x\not\in u\r)&&\textrm{Definition of relative complement}\\
    &\Leftrightarrow x\in v\land\l(x\not\in v\lor x\in u\r)&&\textrm{Negation of }\land\\
    &\Leftrightarrow\l(x\in v\land x\not\in v\r)\lor\l(x\in v\land x\not\in u\r)\ \ \ \ \ \ \ \ &&\textrm{Distribution of }\land\textrm{ over }\lor\\
    &\Leftrightarrow x\in v\land x\in u&&x\in v\land x\not\in v\textrm{ is false}\\
    &\Leftrightarrow x\in v\cap u&&\textrm{Definition of intersection}\\
    &\Leftrightarrow x\in u.&&u\subseteq v\qedin
\end{alignat}$$