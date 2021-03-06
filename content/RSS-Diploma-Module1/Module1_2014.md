title: Royal Statistical Society Graduate Diploma Module 1- 2014 Solutions
date: 2016-04-21

# Paper
[Paper Link](http://www.rss.org.uk/Images/PDF/pro-dev/Exam past papers/2014/rss-grad-diploma-module1-2014.pdf)

# Problem 1

## Problem (i)
\begin{align*}
F(x) &= P(X \leq x\\
&= \sum_{A} P(X \leq x, A)\\
&= P(X \leq x, A) + P(X \leq x, A^c)\\
&= P(X \leq x|A)P(A) + P(X \leq x|A^c)P(A^c)\\
&= F_1(x)\theta + F_2(x)(1-\theta)
 \end{align*}

To deduce the next equation, we simply
differentiate the above:


\begin{align*}
\frac{d}{dx} F(x) &= \frac{d}{dx} F_1(x)\theta+F_2(x)(1-\theta)\\
f(x) &= f_1(x)\theta+f_2(x)(1-\theta)\\
\int x f(x)dx &= \int x\theta f_1(x)dx + \int x(1-\theta)f_2(x)dx\\
E[X] &= \theta \mu_1 + (1-\theta)\mu_2
\end{align*}

## Problem (ii)

\begin{align*}
W_i &\sim \mathcal{N}(4.5,0.25)\\
S_6=\sum_{i=1}^6 W_I &\sim \mathcal{N}(27,1.5)\\
P(S_6\leq 25) &= P(\frac{S_6-27}{\sqrt{1.5}} \leq -\frac{2}{\sqrt{1.5}})\\
&= P(Z \leq -1.63)\\
&=0.056
\end{align*}

## Problem (iii)

\begin{align*}
EW &= P(S_6 \leq 25)E[S_7] + P[S_6 \geq 25]E[S_6]\\
&= 0.056*31.5+(1-0.056)*27\\
&= 27.322
\end{align*}

## Problem (iv)

\begin{align*}
P(S_6 \leq 25) &= 0.01\\
P(Z \leq -\frac{2}{\sigma}) &= 0.01
\implies -\frac{2}{\sigma}&= -2.33\\
&= 1.165
\end{align*}

# Problem 2


## Problem (i)
Median = $\int_{-\infty}^m = \frac{1}{2}$
Thus,
\begin{align*}
\int_{-\infty}^m xf(x) dx &= \frac{1}{2}\\
\int_{-p}^{\infty}
 x f(-x) = \frac{1}{2}\\
&= \int_p^{\infty} xf(x)\\
&=  \int_{-p}^{\infty} xf(-x)dx\\
\implies p &=0
\end{align*}

Thus median $m=0$



## Problem (ii)

\begin{align*}
EX &= \int_{-\infty}^{\infty}xf(x)dx \\
&= \int_{\infty}^{-\infty}-xf(-x)d(-x) \ x \longrightarrow -x\\
&= -\int_{-\infty}^{\infty}xf(-x)dx\\
&= -\int_{-\infty}^{\infty}xf(x)dx \text{ since } f(x)=f(-x) \\
\implies E[X] &=0
\end{align*}

## Problem (iii)

$Y=X^2$

\begin{align*}
E[XY] &= E[X^3]\\
&= \int_{-\infty}^\infty x^3f(x)dx\\
&=0
\end{align*}

$Cov(X<y)=E[XY]-E[X]E[Y] = 0$ and hence $X,Y$ are uncorrelated

## Problem (iv)

\begin{align*}
g(y) &= f_X(\sqrt{y}) \frac{dx}{dy}\\
&= \frac{1}{2\sqrt{y}}f_X(\sqrt{y})\\
\text{Note the typo in the original question where $\frac{1}{2}$ is issing}
\end{align*}

# Problem 3

## Problem 3.(i)
\begin{align*}
f(x,y) &= \frac{1}{x}e^{-x} \\
f(x) &= \int_0^{x} f(x,y)dy\\
&= e^{-x}\\
f_{Y|X}(x)&=\frac{f(X=x,Y)}{f(X)}\\
&= \frac{1}{x}
\end{align*}

## Problem 3.(ii)
\begin{align*}
E[X^mY^n] &= \int_{y}^ix^my^n\frac{1}{x}e^{-x} dxdyi\\
&= \int_0^\infty x^{m-1e^{-xdx} \int_0^x y^mdy}\\
&= \int_0^\infty x^{m-1+n+1}e^{-x}\frac{1}{n}\\
&= \frac{(m+n)!}{n+1}
\end{align*}

## Problem 3.(iii)

\begin{align*}
E[X]&=1\\
E[X^2] &= 2\\
Var(X) &= 1\\
E[Y]&= 1/2\\
E[Y^2] &= 2/3\\
Var(Y) &= 5/12
\end{align*}

# Problem 4

## Problem 4.(i)

\begin{array}{|c|c|c|}
X1/X2 & 0 & 1\\\hline
0 & 0.1 & 0.1\\\hline
1 & 0.3 & 0.5\\\hline
\end{array}


## Problem 4.(ii)
\begin{align*}
S_Y &= \{0, 1, 2, 3\}\\
\end{align*}
Idea: Start of with a random row and column in the table,
Then keep sampling until there are 10 samples(Ignoring anything that is not in $S_Y$)

## Problem 4.(iii)

This is straightforward based on theses caseSs

\begin{align*}
Y&=0 \implies X_1=0,X_2=0\\
Y&=1 \implies X_1=0,X_2=1\\
Y&=2 \implies X_1=1, X_2=0\\
Y&=3 \implies X_1=1,X_2=1
\end{align*}

## Problem 4b

TODO


# Problem 5

## Problem 5.(i)
\begin{align*}
cor(X_1,X_2) &= \frac{Cov(X_1,X_2)}{\sigma_1\sigma_2}\\
&= \frac{2}{4}\\
&= 1/2
\end{align*}

## Problem 5.(ii)

\begin{align*}
E[Y] &= -1+1 =0\\
Var(Y) &= Var(X_1) + Var(X_2) + 2Cov(X_1,X_2)\\
&= 21
\end{align*}


## Problem 5.(ii)
Since $Y_1.Y_2$ are both normal, independnce requires just the covariance being zero.

\begin{align*}
Cov(Y_1,Y_2) &=0\\
&= KVar(X_1)+ (k+1)Cov(X_1,X_2) + Var(X_2)\\
&= 3k+18\\
\implies k &=-6
\end{align*}

## Problem 5.(b)

$E[\mathbf{Y}]=\mathbf{0}$

$V=\begin{pmatrix}
1/3 & 2/9 & 1/9 & 0 & \dots & 0\\
2/9 & 2/9 & 1/9 & 0 & \dots & 0\\
1/9 & 1/9 & 1/9 & 0 & \dots & 0\\
0   & 0   & 0   & 1/3 & 2/9 & 1/9\\
\end{pmatrix}$ 
Essentiall th 3 rows block shifts every 4th row.

Joint distribution of $Y_1,Y_2,\dots, Y_{n-2}$ follows a MVN with mean 0 and variance as the above matrix

# Problem 6
\begin{align*}
M_X(t) &= E[e^{tX}]\\
&= \int_0^\infty \frac{e^{tx} \theta^\alpha x^{\alpha-1} e^{-\theta x}}{\Gamma(\alpha)}dx\\
&= \int_0^\infty \frac{(\theta-t)^\alpha}{(\theta-t)^\alpha} \frac{ \theta^\alpha x^{\alpha-1} e^{t-\theta x}}{\Gamma(\alpha)}\\
&= \frac{\theta^\alpha}{(t-\theta)^\alpha}\\
EX &= M_X'(0)\\
&= \alpha\theta^\alpha(\theta-t)^{-\alpha-1}\\
&= \alpha/\theta\\
EX^2 &= M_X''(0)\\
&= \alpha(\alpha-1)/\theta^2\\
Var(X) = \alpha/\theta^2-\alpha(\alpha-1)/\theta^2\\
&= \alpha/\theta^2
\end{align*}

## Problem 6.(ii)

\begin{align*}
M_X(t) &= \frac{\theta}{\theta-t}
Z &= \sum_iX_i\\
M_Z(t) &= \prod M_{X_i}(t)\\
&= (\frac{\theta}{\theta-t})^n\\
&\sim \Gamma(\theta,n)
\end{align*}

## Problem 6.(iii)

Central Limit Theorem: 

If $X_i$ represent random variables whose mgf exits in a neighborhood of 0
and has finite first and second momements, then $\frac{\bar{X_n}-\mu}{\sigma/\sqrt{n}} \sim \mathcal{N}(0,1)$

$\Gamma(n,\theta) \sim \mathcal{N}(n\sqrt{n}/\theta,n^2/\theta^2 )$

# Problem 7

## Problem 7(a)
\begin{align*}
P[X_1=1] &= \frac{m}{n} \\
P[X_2=1] &= \sum_{{x_1}} P(X_2=1|X_=x_1)P(X_1=x_1)\\
&= \frac{m}{n}*\frac{m-1}{n-1} + \frac{n-m}{n}\frac{m}{n-1}\\
&= \frac{m}{n}\\
P[X_3=1] &= \sum_{{x_1,x_2}} P(X_3=1,X_2=x_2,X_1=x_1)\\
&= \sum_{x_1,x_2} P(X_3=1|X_1=x_1,X_2=x_2)P(X_1=x_1,X_2=x_2)\\
&= \frac{m}{n} \frac{m-1}{n-1} \frac{m-2}{n-2}\\
&+ \frac{m}{n} \frac{n-m}{n-1} \frac{m-1}{n-2}\\
&+ \frac{n-m}{n} \frac{m}{n-1} \frac{m-1}{n-2}\\
&+ \frac{n-m}{n} \frac{n-m-1}{n-1} \frac{m}{n-2}\\
&= \frac{m}{n}\\
P[X_1=1,X_2=1] &= \frac{m(m-1)}{n(n-1)}
\end{align*}


\begin{align*}
E[X_iX_j] &= P(X_i=1,X_j=1)\\
&= \frac{m(m-1)}{n(n-1)} \\
Cov[X_i, X_j] &= E[X_i X_j]-E[X_i]E[X_j]\\
&= \frac{m(m-1)}{n(n-1)} - (\frac{m}{n})^2\\
&= \frac{m(m-n)}{n(n-1)}
\end{align*}

## Problem 7(b)

\begin{align*}
S &= \sum_{i=1}^n I_i\\
Var(S) &= \sum_{i=1}^k Var(I_i) + 2\sum_{i<j} Cov(I_i,I_j)\\
&= k \times (\frac{m}{n}-(\frac{m}{n})^2) + k(k-1) \frac{m(m-n)}{n(n-1)}\\
&= \frac{km}{n} (1-\frac{m}{n} + (k-1))\frac{m-n}{n(n-1)})\\
&= k\frac{m}{n}(1-\frac{m}{n})\frac{n-k}{n-1}\\
\end{align*}



# Problem 8

## Problem 8(a,b)
\begin{align*}
R &= \sqrt{X^2+Y^2}\\
Q &= tan^{-1} (\frac{Y}{X})\\
\begin{vmatrix}
\frac{\partial X}{\partial R} & \frac{\partial X}{\[\partial Q}\\
\frac{\partial Y}{\partial R} & \frac{\partial Y}{\[\partial Q}\\
\end{vmatrix} &= R\\
P(R,Q) &= RP(X(R), Y(Q))\\
&= \frac{R}{2\pi \sigma^2} exp^{-\frac{R^2}{2\sigma^2}}\\
&= \frac{R}{\sigma^2}exp^{-\frac{R^2}{2\sigma^2}} \times \frac{1}{2\pi}\\
&= P(R)P(Q)\\
P(R) &=  \frac{R}{\sigma^2}exp^{-\frac{R^2}{2\sigma^2}}\\
\end{align*}

## Problem 8(c)

\begin{align*}
P(R < k\sigma ) &= 0.5\\
\int_0^{k\sigma} \frac{$R}{\sigma^2} exp^{-\frac{R^2}{2\sigma^2}}dR  &= 0.5
exp^{-\frac{k^2}{2}}&=0.5\\
k^2 &= 2\ln(2)
\end{align*}


