title: Royal Statistical Society Graduate Diploma Module 2- 2014 Solutions
date: 2016-06-06

# Paper

[http://www.rss.org.uk/Images/PDF/pro-dev/Exam%20past%20papers/2014/rss-grad-diploma-module2-2014.pdf](http://www.rss.org.uk/Images/PDF/pro-dev/Exam%20past%20papers/2014/rss-grad-diploma-module2-2014.pdf)

## Problem 1(i)

\begin{align*}
P(V=k) &= p(1-p)^{k-1}\\
G_V(z) &= E[z^V]\\
&= \sum_{k=1} ^\infty z^kp(1-p)^{k-1}\\
&= \frac{p}{1-p} \sum_{k=1} (z(1-p))^k\\
&= \frac{p}{1-p} z(1-p) \frac{1}{1-z(1-p)}\\
&= \frac{zp}{1-z(1-p)}\\
G_W(z) &= \Pi_{i=1}^n G_{V_i}(z)\\
&= (\frac{zp}{1-z(1-p)})^n\\
\end{align*}

## Problem 1(ii)

\begin{align*}
f(X|p) &= p^n(1-p)^{W-n}\\
\log(f(X|p)) &= n \log(p) + (W-n)\log(1-p)\\
\frac{\partial f(X|p)}{\partial p} &= \frac{n}{p} - (W-n)\frac{1}{1-p}\\
\frac{\partial^2 f(X|p)}{\partial p^2} &= -\frac{n}{p^2} - (W-n)\frac{1}{(1-p)^2}\\
\text{Cramer-Rao LB} &= \frac{E[\theta]'}{E[-frac{\partial^2}{\partial p^2}\log(f(X|p))]}\\
&= \frac{1}{E[\frac{n}{p^2} + (W-n)\frac{1}{(1-p)^2}\\ ]}
&= \frac{p^2(1-p)}{n}
\end{align*}
