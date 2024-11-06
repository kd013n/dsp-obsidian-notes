## Item 1
#### Given
$$
x(t) = \begin{cases}
\frac{t}{2}+1, &-2 \le t \le 0 \\
1, &0 \le t \le 2  \\
t-4, &2 \le t \le 4 \\
0, &\text{otherwise}
\end{cases}
$$

#### Solution
##### Time Interval
$$
\begin{gather}
\text{For } -2 \le t \le 0: \\\\
-2 \le t \le 0 \\
-2 \le 2t + 4 \le 0 \\\\
2t + 4 \ge -2 \\
2t \ge -6 \\
t \ge -3 \\\\
2t + 4 \le 0 \\
2t \le -4 \\
t \le -2 \\\\
\boxed{-3 \le t \le -2} \\\\\\
\end{gather}
$$
$$
\begin{gather}
\text{For } 0 \le t \le 2: \\\\
0 \le t \le 2 \\
0 \le 2t + 4 \le 2 \\\\
2t + 4 \ge 0 \\
2t \ge -4 \\
t \ge -2 \\\\
2t + 4 \le 2 \\
2t \le -2 \\
t \le -1 \\\\
\boxed{-2 \le t \le -1} \\\\\\
\end{gather}
$$
$$
\begin{gather}
\text{For } 2 \le t \le 4: \\\\
2 \le t \le 4 \\
2 \le 2t + 4 \le 4 \\\\
2t + 4 \ge 2 \\
2t \ge -2 \\
t \ge -1 \\\\
2t + 4 \le 4 \\
2t \le 0 \\
t \le 0 \\\\
\boxed{-1 \le t \le 0} \\\\\\
\end{gather}
$$
##### For $y(x)$
$$
\begin{gather}
\text{@ } t: (-\infty, -3],\ [0, \infty) \\\\
x(t) = 0 \\\\
y(t) = -2(0) + 3 \\
\boxed{y(t) = 3} \\\\\\
\end{gather}
$$
$$
\begin{gather}
\text{@ } t: [-3, -2] \\\\
\text{For } t = -3: \\
2(-3) + 4 = -6 + 4 = -2 \\\\
x(t) = \frac{t}{2} + 1 \\\\
y(t) = -2 \left[\frac{(2t+4)}{2} + 1\right] + 3 \\
y(t) = -2(t+2+1) +3 \\
y(t) = -2(t+3) +3 \\
y(t) = -2t - 6 + 3 \\
\boxed{y(t) = -2t - 3} \\\\\\
\end{gather}
$$
$$
\begin{gather}
\text{@ } t: [-2, -1] \\\\
\text{For } t = -1: \\
2(-1) + 4 = -2 + 4 = 2 \\\\
x(t) = 1 \\
\boxed{y(t) = 1} \\\\\\
\end{gather}
$$
$$
\begin{gather}
\text{@ } t: [-1, 0] \\\\
\text{For } t = 0: \\
2(0) + 4 = 4 \\\\
x(t) = t - 4 \\\\
y(t) = -2 [(2t + 4) - 4] + 3 \\
y(t) = -2(2t) + 3 \\
\boxed{y(t) = -4t + 3} \\\\\\
\end{gather}
$$
#### Final Answer
$$
y(t) = \begin{cases}
3, &t \le -3 \\
-2t - 3, &-3 \le t \le -2 \\
1, &-2 \le t \le -1 \\
-4t + 3, &-1 \le t \le 0 \\
3, &t \ge 0
\end{cases}
$$

## Item 2
#### Given
$$
y[n] = 2x[n+1] - x[-2n]
$$
#### Solution
$$
\begin{gather}
\text{For } 2x[n+1]: \\
x[n] = [\underset{\uparrow}{3},\ 3,\ 2,\ 1,\ 1] \\
x[n + 1] = [3,\ 3,\ \underset{\uparrow}{2},\ 1,\ 1] \\
2x[n + 1] = [6,\ \underset{\uparrow}{6},\ 4,\ 2,\ 2] \\
\end{gather}
$$
$$
\begin{gather}
\text{For } x[-2n]: \\
x[n] = [\underset{\uparrow}{3},\ 3,\ 2,\ 1,\ 1] \\
x[-n] = [1,\ 1,\ 2,\ 3,\ \underset{\uparrow}{3}] \\
x[-2n] = [1,\ 2,\ \underset{\uparrow}{3}] \\
\end{gather}
$$
$$
\begin{gather}
\text{For } 2x[n+1] - x[-2n]: \\
2x[n + 1] = [6,\ \underset{\uparrow}{6},\ 4,\ 2,\ 2] \\
x[-2n] = [1,\ 2,\ \underset{\uparrow}{3}] \\\
\boxed{2x[n+1] - x[-2n] = [-1,\ 4,\ \underset{\uparrow}{3},\ 4,\ 2,\ 2]}
\end{gather}
$$
#### Final Answer
$$
\begin{gather}
2x[n+1] - x[-2n] = [-1,\ 4,\ \underset{\uparrow}{3},\ 4,\ 2,\ 2]
\end{gather}
$$