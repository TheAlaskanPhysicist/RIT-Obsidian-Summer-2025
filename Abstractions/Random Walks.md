
Let probabilities $\vec{p}=\left(p_1,p_2,\dots,p_d\right)$ exist for displacements $\Delta\vec{x}=\left(\Delta x_1,\Delta x_2,\dots,\Delta x_d\right)$, such that:
$$\begin{align}
\sum_kp_k&=1
\end{align}$$
We can define the Probability Density Function as:
$$\begin{align}
\text{PDF}(S, k)&=\sum_{\vec{s}\in P(S,k)}\dfrac{S!}{s_1!s_2!\dots s_d!}p_1^{s_1}p_2^{s_2}\dots p_d^{s_d}\\
P(S,k)&=\left\{\vec{s}\ |\ \left(\sum_{i}s_i=S\right) \land \left(\vec{s}\cdot\Delta\vec{x}=k\right) \right\}
\end{align}$$
To find the CDF in $k$, we see that:
$$\begin{align}
\text{CDF}_k(S, k)&=\sum_{i\lt k}\text{PDF}(S, i) && \text{(Prob. of }S\text{ steps taking}<k\text{ displacement)}\\
1-\text{CDF}_k(S, k)&=\sum_{i\ge k}\text{PDF}(S, i) && \text{(Prob. of }S\text{ steps taking}\ge k\text{ displacement)}\\
\end{align}$$
To find the CDF in $S$, we see that:
$$\begin{align}
\text{CDF}_s(S, k)&=\sum_{s\le S}\text{PDF}(s, k) && \text{(Prob. of displacement }k\text{ in }S\text{ or less steps.)}\\
1-\text{CDF}_s(S, k)&=\sum_{s\gt S}\text{PDF}(s, k) && \text{(Prob. of displacement }k\text{ in }S+1\text{ and greater steps.)}\\
\end{align}$$




---
### Eni's Problem
To find the probability of the displacement $x\le -X_0$, fixing the number of steps $S$, we find:
$$\begin{align}
p(x\le-X_0 \ |\ S)&=\sum_{x\le -X_0}\text{PDF}(S, x)
\end{align}$$
Where:
$$\begin{align}
\text{PDF}(S, x)&=\sum_{\vec{s}\in P(S,x)}\dfrac{S!}{s_1!s_2!\dots s_d!}p_1^{s_1}p_2^{s_2}\dots p_d^{s_d}\\
P(S,x)&=\left\{\vec{s}\ |\ \left(\sum_{i}s_i=S\right) \land \left(\vec{s}\cdot\Delta\vec{x}=x\right) \right\}
\end{align}$$
Consequently, we can rewrite this in a singular condition as:
$$\begin{align}
p(x\le-X_0 \ |\ S)&=\sum_{\vec{s}\in C(S,-X_0)}\dfrac{S!}{s_1!s_2!\dots s_d!}p_1^{s_1}p_2^{s_2}\dots p_d^{s_d}\\
C(S,-X_0)&=\left\{\vec{s}\ |\ \left(\sum_{i}s_i=S\right) \land \left(\vec{s}\cdot\Delta\vec{x}\le -X_0\right) \right\}
\end{align}$$
---
$$\begin{align}
p(x\le-X_0)&=\sum_{s=0}^S\sum_{\vec{s}\in C(s,-X_0)}\dfrac{s!}{s_1!s_2!\dots s_d!}p_1^{s_1}p_2^{s_2}\dots p_d^{s_d}\\
C(S,-X_0)&=\left\{\vec{s}\ |\ \left(\sum_{i}s_i=S\right) \land \left(\vec{s}\cdot\Delta\vec{x}\le -X_0\right) \right\}
\end{align}$$














$$\begin{align}

\end{align}$$
The expected number of steps is a little weird since you need to account for permutations with the step number since there is early termination.
$$\begin{align}
\mathbb{E}(N)_{\Delta x}=X_0P(X_0)+(X_0+1)\left(P(X_0+1)-P(X_0)\right)+(X_0+2)\left(P(X_0+2)-P(X_0+1)-P(X_0)\right)+\dots
\end{align}$$
We can write this in summation notation:
$$\begin{align}
\mathbb{E}(N)&=\sum_{n\ge1} n\left(2P(n)-\sum_{k=0}^{n}P(k)\right)\\
\end{align}$$
We can note that the following relationship is true:
$$\begin{align}

\end{align}$$