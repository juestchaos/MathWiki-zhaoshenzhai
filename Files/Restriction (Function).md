<br />
<br />

Date Created: 26/01/2022 17:46:40
Tags: #Definition #Closed 

Constructions: _Not Applicable_
Generalizations: [[Restriction (Relation)]]

Types: _Not Applicable_
Examples: [[Inclusion Function]]
Properties: [[Restriction of function is a function]]

!!! ad-Definition Definition.

Let $f:X\to Y$ and fix $S\subseteq X$. The **restriction of $f$ to $S$** is the function
$$\begin{equation}
    \l.f\r|_S:S\to Y\ \ \ \ \textrm{mapping}\ \ \ \ x\mapsto f\l(x\r)
\end{equation}$$
for all $x\in S$. Formally,
$$\begin{equation}
    \l.f\r|_S\coloneqq\l\{z\mid\ex x\in S:z=\l\langle x,f\l(x\r)\r\rangle\r\}.
\end{equation}$$

--- admonition

**Remark.** Note that $\l.f\r|_S$ is also the restriction of $f$, _viewed as a relation_, since
$$\begin{align}
    \l.f\r|_S&=\l\{z\mid\ex x\in S:x=\l\langle x,f\l(x\r)\r\rangle\r\}\\
    &=\l\{z\mid\ex x:x\in S\land z=\l\langle x,f\l(x\r)\r\rangle\r\}\\
    &=\l\{z\mid\ex x:z=\l\langle x,f\l(x\r)\r\rangle\land x\in S\r\}\\
    &=\l\{z\mid\ex x,y:z=\l\langle x,y\r\rangle\land z\in f\land x\in S\r\}\\
    &=\l\{z\in f\mid\ex x,y:z=\l\langle x,y\r\rangle\land x\in S\r\}\\
    &=f\rest S.\exqedin
\end{align}$$