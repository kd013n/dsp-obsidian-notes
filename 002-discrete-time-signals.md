### Footnotes
 $e^{j \theta}=\cos(\theta)+j \sin(\theta)$
$\lim(f(x))$

### Classifications of DTS
- Periodic - Rational FTP value (fraction)
- Aperiodic - Irrational FTP value (fraction w/ pi)
### Fundamental Time Period
##### Formula for **Fundamental Time Period**
$$\begin{gather}
T = \frac{2\pi}{\omega} \qquad \text{or} \qquad N = \frac{2\pi}{\omega}
\end{gather}$$
where:
$T$ = Fundamental Time Period (continuous)
$N$ = Fundamental Time Period (discrete)
$\omega$ = Angular Frequency $(2\pi f)$

##### Formula for Fundamental Time Period ($T_{1,} \ T_{2}$)

$$\begin{gather}
\text{Determine the ratio} \\\\
\frac{T_{1}}{T_{2}} \\\\\\
\text{If rational (periodic):} \\\\
T = \frac{LCM_{a}}{GCF_{b}} \quad \text{for} \quad T_{n}= \frac{a}{b} \\\\
\text{* note: T for continuous, N for discrete}
\end{gather}$$

#### Worked Examples

>[!example]+ Example 1
>> [!abstract] Given
>> $$
\begin{gather}
x(n) = e^{j5n}
\end{gather}
>> $$
>
>> [!done] Solution
>> $$
\begin{gather}
x(n) = \cos{5n} + j\sin{5n} \\
\omega = 5 \\\\
N = \frac{2\pi}{\omega} \\\\
N = \frac{2\pi}{5} \; \rightarrow \; \text{irrational} \\
\boxed{\therefore \ N = \frac{2\pi}{5}, \; \text{Aperiodic}}
\end{gather}
>> $$
>

>[!example]+ Example 2
>> [!abstract] Given
>> $$
\begin{gather}
x(n) = \sin{\left(\frac{5\pi}{7}n\right)}
\end{gather}
>> $$
>
>> [!done] Solution
>>$$
\begin{gather}
\omega = \frac{5\pi}{7} \\\\\\
N = \frac{2\pi}{\omega} \\\\
N = \frac{2\pi}{\frac{5\pi}{7}} = 2\pi \times \frac{7}{5\pi} \\\\
N = \frac{14}{5} \ \rightarrow \ \text{rational}\\\\
\boxed{\therefore \ N = 2.8, \  \text{Periodic}}
\end{gather}
>>$$

>[!example]+ Example 3
>> [!abstract] Given
>> $$
\begin{gather}
x(t) = \sin{6\pi t}+\cos{5\pi t}
\end{gather}
>> $$
>
>> [!done] Solution
>>$$
\begin{gather}
\omega_{1} = 6\pi \quad \omega_{2} = 5\pi \\\\\\
T_{1} = \frac{2\pi}{6\pi} = \frac{1}{3} \\\\
T_{2} = \frac{2\pi}{5\pi} = \frac{2}{5} \\\\\\
\text{For the ratio:} \\
\frac{T_{1}}{T_{2}} = \frac{\frac{1}{3}}{\frac{2}{5}} = \frac{1}{3} \times \frac{5}{2} \\\\
\frac{T_{1}}{T_{2}} = \frac{5}{6} \ \rightarrow \ \text{rational} \\\\\\
\text{Since the ratio is rational:} \\\\
T = \frac{LCM_{num}}{GCF_{denum}} \\\\
T = \frac{2}{1} \\\\
\boxed{\therefore \ T = 2, \; \text{Periodic}}
\end{gather}
>>$$

### Energy and Power Signals
#### Infinite Sequence
##### Normalized energy $(E)$ of $x(t)$
$$\begin{gather}
E = \lim_{L\to\infty} \int^{L}_{-L} [x(t)]^{2}
\end{gather}

$$
##### Normalized power $(P)$ of $x(t)$
$$\begin{gather}
P = \lim_{L\to\infty} \frac{1}{2L} \int^{L}_{-L} [x(t)]^{2}
\end{gather}$$


>[!example]+ Example 1
>> [!abstract] Given
>> $$ x(t) = \begin{cases}
e^{-t} &; \; t \ge 0 \\
0 &; \; \text{otherwise}
\end{cases}
>>$$
>
>> [!done] Solution
>> $$ \begin{gathered}
\text{As an energy signal:} \\\\
E = \lim_{L\to\infty} \int_{-L}^{L} [x(t)]^{2} \ dt \\\\
E = \lim_{L\to\infty} \left\{ \int_{0}^{L} [e^{-t}]^{2}\ dt \; + \; \int_{-L}^{0} [0]^{2} \ dt \right\} \\\\
E = \lim_{L\to\infty} \int_{0}^{L} e^{-2t} \ dt \\\\
E = \lim_{L\to\infty} \left[ -\frac{1}{2} e^{-2t} \right]_{0}^{L} \\\\
E = \lim_{L\to\infty} \left\{-\frac{1}{2} e^{-2L} - \left( -\frac{1}{2} e^{-2(0)} \right)\right\} \\\\
E = -\frac{1}{2} e^{-\infty} - \left( -\frac{1}{2} e^{0} \right)\\\\
E = 0 - \left( -\frac{1}{2} \right) \\\\
\boxed{E = \frac{1}{2}} \\\\\\\\
\text{As a power signal:} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \int^{L}_{-L} [x(t)]^{2} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \int_{0}^{L} [e^{-t}]^{2}\ dt \; + \; \int_{-L}^{0} [0]^{2} \ dt \right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \int^{L}_{0} e^{-2t} \ dt \; + \int^{0}_{-\infty} 0 \ dt \right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \int^{L}_{0} e^{-2t} \ dt \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left[ -\frac{1}{2}e^{-2t} \right]_{0}^{L} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ -\frac{1}{2}e^{-2L} - \left( -\frac{1}{2}e^{-2(0)} \right) \right\} \\\\
\text{note: } \lim_{x \rightarrow \infty} \frac{1}{x} = 0\\\\
P = 0 \left[ -\frac{1}{2}e^{-\infty} - \left( -\frac{1}{2}e^{-2(0)} \right) \right] \\\\
\boxed{P = 0} \\\\
\boxed{\therefore \text{The signal is an energy signal since} \; E = \frac{1}{2}}
\end{gathered}
>$$

>[!example]+ Example 2
>> [!abstract] Given
>> $$ x(t) = \begin{cases}
1 &; \; t \le 0 \\
e^{-t} &; \; t \ge 0
\end{cases}
>>$$
>
>> [!done] Solution
>> $$ \begin{gathered}
\text{As an energy signal:} \\\\
E = \lim_{L\to\infty} \int_{-L}^{L} [x(t)]^{2} \ dt \\\\
E = \lim_{L\to\infty} \left\{ \int^{0}_{-L} [1]^{2}\ dt \; + \int^{L}_{0} [e^{-t}]^{2} \right\} \\\\
E = \lim_{L\to\infty} \left\{ \int^{0}_{-L} dt \; + \int^{L}_{0} e^{-2t} \right\} \\\\
E = \lim_{L\to\infty} \left\{ \left[t\right]_{-L}^{0} \; + \left[-\frac{1}{2} e^{-2t}\right]_{0}^{L}\right\} \\\\
E = \lim_{L\to\infty} \left\{ \left[0-(-L)\right] \; + \left[-\frac{1}{2} e^{-2L} - \left(-\frac{1}{2} e^{-2(0)}\right)\right] \right\}\\\\
E = \left[0-(-\infty)\right] \; + \left[-\frac{1}{2} e^{-\infty} - \left(-\frac{1}{2} e^{0}\right)\right]\\\\
E = \infty \ + \ 0 \ + \ \frac{1}{2} \\\\
\boxed{E = \infty} \\\\\\
\text{As an power signal:} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \int^{L}_{-L} [x(t)]^{2} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \int^{0}_{-L} [1]^{2}\ dt \; + \int^{L}_{0} [e^{-t}]^{2} \right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \int^{0}_{-L} dt \; + \int^{L}_{0} e^{-2t} \right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \left[t\right]_{-L}^{0} \; + \left[-\frac{1}{2} e^{-2t}\right]_{0}^{L}\right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \left[t\right]_{-L}^{0} \; + \left[-\frac{1}{2} e^{-2t}\right]_{0}^{L}\right\} \\\\
P = \lim_{L\to\infty} \frac{1}{2L} \left\{ \left[0-(-L)\right] \; + \left[-\frac{1}{2} e^{-2L} - \left(-\frac{1}{2} e^{-2(0)}\right)\right] \right\} \\\\
P = \lim_{L\to\infty} \frac{L}{2L} - \lim_{L\to\infty} \frac{e^{-2L}}{4L} +\lim_{L\to\infty} \frac{1}{4L} \\\\
P = \frac{1}{2} - \frac{0}{\infty} + \frac{1}{\infty} \\\\
P = \frac{1}{2} - 0 + 0 \\\\
\boxed{P = \frac{1}{2}} \\\\\\
\boxed{\therefore \text{The signal is a power signal since} \; P = \frac{1}{2}}
\end{gathered}
>$$

#### Finite Sequence
##### Normalized energy $(E)$ of $x(n)$
$$\begin{gather}
E = \displaystyle\sum_{n=-\infty}^{\infty} {\lvert x(n) \rvert}^2
\end{gather}
$$

##### Normalized power $(P)$ of $x(n)$
$$\begin{gather}
P = \lim_{L\to\infty} \frac{1}{N_{2}- N_{1}+ 1} \sum^{N_2}_{n=N_{1}} {\lvert x(n) \rvert}^{2} \\\\
\text{where:} \\ N_{1} = \text{lower bound} \\ N_{2}= \text{upper bound} 
\end{gather}$$


>[!example]+ Example 1
>> [!abstract] Given
>> $$ \begin{gather}
x(t) = \left\{1, 0, -3, -2, 0, -2\right\}
\end{gather}
>>$$
>
>> [!done] Solution
>> $$ \begin{gathered}
\text{As an energy signal:} \\\\
E = \displaystyle\sum_{n=-\infty}^{\infty}  [x(n)]^{2} \\\\
E = (1)^{2} + (0)^{2} + (-3)^{2} + (-2)^{2} + (0)^{2} + (-2)^{2}\\\\
E = 1 + 0 + 9 + 4 + 0 + 4 \\\\
\boxed{E = 18} \\\\\\
\text{As an power signal:} \\\\
P = \lim_{L\to\infty} \frac{1}{N_{2}- N_{1}+ 1} \sum^{N_2}_{n=N_{1}} {\lvert x(n) \rvert}^{2} \\\\
\boxed{P = \frac{1}{2}} \\\\\\
\boxed{\therefore \text{The signal is a power signal since} \; P = \frac{1}{2}}
\end{gathered}
>$$