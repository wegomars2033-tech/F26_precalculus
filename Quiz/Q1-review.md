---
geometry: margin=0.5in
fontsize: 10pt
---

# Quiz 1 Review: Formulas from Lectures 1–7

**Fall 2026 Precalculus.** Angles are in radians unless a degree symbol
appears, and $k\in\mathbb Z$ means $k$ is any integer.

## Lecture 1: Coordinates, Lines, and Circles

| Idea | Formula |
|:--|:--|
| Distance from $(x_1,y_1)$ to $(x_2,y_2)$ | $d=\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}$ |
| Midpoint | $M=\left(\dfrac{x_1+x_2}{2},\ \dfrac{y_1+y_2}{2}\right)$ |
| Circle with center $(h,k)$ and radius $r$ | $(x-h)^2+(y-k)^2=r^2$ |
| Slope ($x_1\neq x_2$) | $m=\dfrac{y_2-y_1}{x_2-x_1}$ |
| Point-slope form | $y-y_1=m(x-x_1)$ |
| Slope-intercept form | $y=mx+b$ |
| General form (includes vertical lines) | $Ax+By+C=0$, with $A,B$ not both $0$ |
| Parallel lines | $m_1=m_2$ |
| Perpendicular lines | $m_1m_2=-1$, so the new slope is $-1/m$ |
| Intersection of $y=m_1x+b_1$ and $y=m_2x+b_2$ | $x=\dfrac{b_2-b_1}{m_1-m_2}$ when $m_1\neq m_2$ |
| Centroid of a triangle | $G=\left(\dfrac{x_1+x_2+x_3}{3},\ \dfrac{y_1+y_2+y_3}{3}\right)$ |
| Altitude from a vertex | line through the vertex with slope $-1/m$, where $m$ is the slope of the opposite side |

Slope sign: $m>0$ rises, $m<0$ falls, $m=0$ is horizontal, and an
undefined slope is vertical. The orthocenter is where the three altitudes
meet.

## Lecture 2: Functions, Graphs, and Transformations

**Parent functions.**

| Function | $y=x$ | $y=x^2$ | $y=x^3$ | $y=1/x$ | $y=\sqrt x$ | $y=\lvert x\rvert$ |
|:--|:-:|:-:|:-:|:-:|:-:|:-:|
| Domain | $\mathbb R$ | $\mathbb R$ | $\mathbb R$ | $x\neq0$ | $[0,\infty)$ | $\mathbb R$ |
| Range | $\mathbb R$ | $[0,\infty)$ | $\mathbb R$ | $y\neq0$ | $[0,\infty)$ | $[0,\infty)$ |
| Symmetry | odd | even | odd | odd | neither | even |

**Even and odd.** $f$ is even if $f(-x)=f(x)$ (symmetric about the
$y$-axis) and odd if $f(-x)=-f(x)$ (symmetric about the origin).

**Transformations.** A point $(a,b)$ on $y=f(x)$ moves as follows.

| New function | New point | Effect |
|:--|:--|:--|
| $f(x)+k$ | $(a,\ b+k)$ | shift up $k$ |
| $f(x-h)$ | $(a+h,\ b)$ | shift right $h$ |
| $-f(x)$ | $(a,\ -b)$ | reflect across the $x$-axis |
| $f(-x)$ | $(-a,\ b)$ | reflect across the $y$-axis |
| $af(x)$ | $(a,\ ab)$ | vertical scale by $a$ |

**Quadratics.** $y=a(x-h)^2+k$ has vertex $(h,k)$ and opens up if $a>0$,
down if $a<0$. For $y=ax^2+bx+c$, complete the square:
$$
h=-\frac{b}{2a},\qquad k=c-\frac{b^2}{4a}=f(h).
$$
**Cubics.** $y=a(x-h)^3+k$ has no turning points. **Composition.**
$(f\circ g)(x)=f(g(x))$: apply $g$ first, then $f$.

**Inverse functions.** $f^{-1}$ exists exactly when $f$ is one-to-one
(horizontal line test). Then $f^{-1}(f(x))=x$ and $f(f^{-1}(x))=x$, and
the graph of $f^{-1}$ is the reflection of the graph of $f$ across $y=x$.

\newpage

## Lecture 3: Exponential Functions

**Laws of exponents** ($b,c>0$):
$$
b^mb^n=b^{m+n},\qquad \frac{b^m}{b^n}=b^{m-n},\qquad (b^m)^n=b^{mn},
\qquad (bc)^n=b^nc^n,
$$
$$
b^0=1,\qquad b^{-m}=\frac1{b^m},\qquad b^{p/q}=\sqrt[q]{b^p}.
$$

**Graph of $y=b^x$** ($b>0$, $b\neq1$): domain $(-\infty,\infty)$, range
$(0,\infty)$, passes through $(0,1)$, horizontal asymptote $y=0$.
Increasing if $b>1$, decreasing if $0<b<1$. Also
$\left(\frac1b\right)^x=b^{-x}$, the reflection of $b^x$ across the
$y$-axis.

**The number $e$.** $e=\displaystyle\lim_{n\to\infty}\left(1+\frac1n\right)^n\approx2.71828$.

| Model | Formula |
|:--|:--|
| Compound interest, $n$ times per year | $A(t)=P\left(1+\dfrac rn\right)^{nt}$ |
| Continuous compounding | $A(t)=Pe^{rt}$ |
| Percentage rate per period | $P(t)=P_0(1+r)^t$: growth if $r>0$, decay if $-1<r<0$ |
| Half-life $h$ | $A(t)=A_0\left(\dfrac12\right)^{t/h}$ |
| Doubling time $d$ | $P(t)=P_0\cdot2^{t/d}$ |

The transformation rules from Lecture 2 apply to $y=b^x$. A vertical shift
$k$ moves the horizontal asymptote to $y=k$.

## Lecture 4: Inverse and Logarithmic Functions

**Finding an inverse.** Write $y=f(x)$, solve for $x$, swap $x$ and $y$,
and state any domain restriction. The domains and ranges swap:
$$
\operatorname{dom}(f^{-1})=\operatorname{range}(f),\qquad
\operatorname{range}(f^{-1})=\operatorname{dom}(f).
$$

**Definition** ($b>0$, $b\neq1$, $x>0$):
$$
\log_bx=y\quad\Longleftrightarrow\quad b^y=x.
$$
$\log x$ means $\log_{10}x$ and $\ln x$ means $\log_ex$. Inverse pairs:
$\log_b(b^x)=x$ and $b^{\log_bx}=x$, so $\ln(e^x)=x$ and $e^{\ln x}=x$.
Special values: $\log_b1=0$ and $\log_bb=1$.

| Rule | Formula |
|:--|:--|
| Product | $\log_b(MN)=\log_bM+\log_bN$ |
| Quotient | $\log_b\left(\dfrac MN\right)=\log_bM-\log_bN$ |
| Power | $\log_b(M^r)=r\log_bM$ |
| Change of base | $\log_bC=\dfrac{\ln C}{\ln b}=\dfrac{\log C}{\log b}$ |
| Exponential equation | $a^x=C\ \Longrightarrow\ x=\dfrac{\ln C}{\ln a}$ |
| Time in $A=Pe^{rt}$ | $t=\dfrac{\ln(A/P)}{r}$ |

**Solving log equations.** Find the domain first (every argument must be
positive), combine the logs, then **check every candidate** in the
original equation and reject extraneous ones.

**Graph of $y=\log_bx$:** domain $(0,\infty)$, range $(-\infty,\infty)$,
$x$-intercept $(1,0)$, vertical asymptote $x=0$. For
$y=A\log_b(x-h)+k$, the domain is $x>h$ and the vertical asymptote is
$x=h$. The vertical shift $k$ does not move the asymptote.

**Applications:** $\mathrm{pH}=-\log_{10}[\mathrm H^+]$, decibels
$L=10\log_{10}(I/I_0)$, and Richter magnitude $M=\log_{10}(A/A_0)$.

\newpage

## Lecture 5: Angles and Trigonometric Functions

**Right triangles.** $\sin\theta=\dfrac{\text{opp}}{\text{hyp}}$,
$\cos\theta=\dfrac{\text{adj}}{\text{hyp}}$,
$\tan\theta=\dfrac{\text{opp}}{\text{adj}}$. Special triangles have side
ratios $1:1:\sqrt2$ ($45^\circ$-$45^\circ$-$90^\circ$) and $1:\sqrt3:2$
($30^\circ$-$60^\circ$-$90^\circ$).

**Angle measure.** $180^\circ=\pi$ radians. To convert degrees to
radians, multiply by $\dfrac{\pi}{180}$; to convert radians to degrees,
multiply by $\dfrac{180}{\pi}$. Coterminal angles: $\theta+2k\pi$ (or
$\theta+360^\circ k$).

**Arc length and sector area** ($\theta$ in radians):
$$
s=r\theta,\qquad A=\tfrac12r^2\theta.
$$

**Any angle.** For a point $(x,y)$ on the terminal side, with
$r=\sqrt{x^2+y^2}$:
$$
\sin\theta=\frac yr,\quad\cos\theta=\frac xr,\quad\tan\theta=\frac yx,\qquad
\csc\theta=\frac ry,\quad\sec\theta=\frac rx,\quad\cot\theta=\frac xy.
$$
On the unit circle, $(\cos\theta,\sin\theta)=(x,y)$.

**Special angles.**

| $\theta$ | $0$ | $\pi/6=30^\circ$ | $\pi/4=45^\circ$ | $\pi/3=60^\circ$ | $\pi/2=90^\circ$ |
|:--|:-:|:-:|:-:|:-:|:-:|
| $\sin\theta$ | $0$ | $\dfrac12$ | $\dfrac{\sqrt2}2$ | $\dfrac{\sqrt3}2$ | $1$ |
| $\cos\theta$ | $1$ | $\dfrac{\sqrt3}2$ | $\dfrac{\sqrt2}2$ | $\dfrac12$ | $0$ |
| $\tan\theta$ | $0$ | $\dfrac{\sqrt3}3$ | $1$ | $\sqrt3$ | undefined |

**Signs (ASTC: All Students Take Calculus).** Quadrant I: all positive.
II: $\sin$ (and $\csc$) positive. III: $\tan$ (and $\cot$) positive.
IV: $\cos$ (and $\sec$) positive.

**Reduction by symmetry** to the acute angle $\alpha$:

| Quadrant | $\alpha$ | $\sin\theta$ | $\cos\theta$ | $\tan\theta$ |
|:-:|:-:|:-:|:-:|:-:|
| II | $\pi-\theta$ | $\sin\alpha$ | $-\cos\alpha$ | $-\tan\alpha$ |
| III | $\theta-\pi$ | $-\sin\alpha$ | $-\cos\alpha$ | $\tan\alpha$ |
| IV | $2\pi-\theta$ | $-\sin\alpha$ | $\cos\alpha$ | $-\tan\alpha$ |

**Basic identities.**
$$
\sin^2\theta+\cos^2\theta=1,\qquad 1+\tan^2\theta=\sec^2\theta,\qquad
1+\cot^2\theta=\csc^2\theta,
$$
$$
\tan\theta=\frac{\sin\theta}{\cos\theta},\quad
\csc\theta=\frac1{\sin\theta},\quad
\sec\theta=\frac1{\cos\theta},\quad
\cot\theta=\frac{\cos\theta}{\sin\theta},
$$
$$
\sin(-\theta)=-\sin\theta,\quad\cos(-\theta)=\cos\theta,\quad
\tan(-\theta)=-\tan\theta,\qquad
\sin\left(\tfrac\pi2-\theta\right)=\cos\theta,\quad
\cos\left(\tfrac\pi2-\theta\right)=\sin\theta.
$$
Sine and cosine have period $2\pi$ and values in $[-1,1]$; tangent has
period $\pi$.

\newpage

## Lecture 6: Trigonometric Functions and Their Properties

**Triangles.** With side $a$ opposite angle $A$, and so on:
$$
\text{Sine law: }\frac{a}{\sin A}=\frac{b}{\sin B}=\frac{c}{\sin C},
\qquad
\text{Cosine law: }a^2=b^2+c^2-2bc\cos A.
$$

**Graphs of sine and cosine.**

| | $y=\sin x$ | $y=\cos x$ |
|:--|:--|:--|
| Zeros | $x=k\pi$ | $x=\pi/2+k\pi$ |
| Maximum $1$ at | $x=\pi/2+2k\pi$ | $x=2k\pi$ |
| Minimum $-1$ at | $x=3\pi/2+2k\pi$ | $x=\pi+2k\pi$ |
| Symmetry | odd | even |

They are shifts of each other: $\cos x=\sin(x+\pi/2)$.

**Tangent and reciprocal functions.**

| Function | Asymptotes (excluded $x$) | Range | Period | Symmetry |
|:--|:--|:--|:-:|:-:|
| $\tan x$ | $\pi/2+k\pi$ | $\mathbb R$ | $\pi$ | odd |
| $\cot x$ | $k\pi$ | $\mathbb R$ | $\pi$ | odd |
| $\sec x$ | $\pi/2+k\pi$ | $(-\infty,-1]\cup[1,\infty)$ | $2\pi$ | even |
| $\csc x$ | $k\pi$ | $(-\infty,-1]\cup[1,\infty)$ | $2\pi$ | odd |

**Sinusoids** $y=A\sin(B(x-C))+D$ and $y=A\cos(B(x-C))+D$. Factor the
input first, for example $2x-\frac\pi2=2\left(x-\frac\pi4\right)$.

| Feature | Value |
|:--|:--|
| Amplitude | $\lvert A\rvert$ |
| Period | $T=\dfrac{2\pi}{\lvert B\rvert}$ |
| Phase shift | $C$ to the right |
| Midline and range | $y=D$ and $[D-\lvert A\rvert,\ D+\lvert A\rvert]$ |

**Five-point method** ($B>0$): mark $x=C,\ C+T/4,\ C+T/2,\ C+3T/4,\ C+T$.

| $x$ | $C$ | $C+T/4$ | $C+T/2$ | $C+3T/4$ | $C+T$ |
|:--|:-:|:-:|:-:|:-:|:-:|
| $A\sin(B(x-C))+D$ | $D$ | $D+A$ | $D$ | $D-A$ | $D$ |
| $A\cos(B(x-C))+D$ | $D+A$ | $D$ | $D-A$ | $D$ | $D+A$ |

**Tangent transformed.** $y=A\tan(B(x-C))+D$ has period $\pi/\lvert B\rvert$,
range $\mathbb R$, no amplitude, and asymptotes where
$B(x-C)=\pi/2+k\pi$.

\newpage

## Lecture 7: Trigonometric Transformations, Equations, and Identities

**Point mapping.** For $y=Af(B(x-C))+D$, a point $(u,v)$ on $y=f(x)$
moves to $\left(C+\dfrac uB,\ D+Av\right)$.

**Solving equations.** Treat the whole inner angle as $u$, find all
solutions for $u$, then solve for $x$ (scale the $k$ term too). Restrict
to an interval only at the end.

| Equation | All solutions, $k\in\mathbb Z$ |
|:--|:--|
| $\sin u=\sin\alpha$ | $u=\alpha+2k\pi$ or $u=\pi-\alpha+2k\pi$ |
| $\cos u=\cos\alpha$ | $u=\alpha+2k\pi$ or $u=-\alpha+2k\pi$ |
| $\tan u=\tan\alpha$ | $u=\alpha+k\pi$ |

**Sum and difference formulas.**

| | Sum | Difference |
|:--|:--|:--|
| Sine | $\sin(a+b)=\sin a\cos b+\cos a\sin b$ | $\sin(a-b)=\sin a\cos b-\cos a\sin b$ |
| Cosine | $\cos(a+b)=\cos a\cos b-\sin a\sin b$ | $\cos(a-b)=\cos a\cos b+\sin a\sin b$ |
| Tangent | $\tan(a+b)=\dfrac{\tan a+\tan b}{1-\tan a\tan b}$ | $\tan(a-b)=\dfrac{\tan a-\tan b}{1+\tan a\tan b}$ |

**Double-angle formulas.**
$$
\sin(2x)=2\sin x\cos x,\qquad
\cos(2x)=\cos^2x-\sin^2x=2\cos^2x-1=1-2\sin^2x,\qquad
\tan(2x)=\frac{2\tan x}{1-\tan^2x}.
$$

**Rewriting squares.**
$$
\sin^2x=\frac{1-\cos(2x)}2,\qquad \cos^2x=\frac{1+\cos(2x)}2.
$$

When an equation has a common factor such as $\sin x$, factor it out
instead of dividing by it, or you lose the solutions where that factor
is $0$.
