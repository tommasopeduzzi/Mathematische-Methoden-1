# Aufgabenblatt 3

[[Aufgabenblatt 3.pdf]]

### Aufgabe 1

a)

$\begin{pmatrix}
10 \\
7
\end{pmatrix} = \frac{10*9*8*7*6*5*4}{7*6*5*4*3*2} = \frac{10*9*8}{3*2}=120$

$\begin{pmatrix}
101 \\
99
\end{pmatrix}= \frac{101*100}{2} = 5050$

$\begin{pmatrix}
7 \\
3
\end{pmatrix} = \frac{7*6*5}{3*2} = 35$

$\begin{pmatrix}16 \\
4
\end{pmatrix} = 2*5*14*13= 1820$

b)

$\begin{pmatrix}
8 \\
3
\end{pmatrix} = \frac{8*7*6}{3*2} = 56$

$\begin{pmatrix}8 \\
4
\end{pmatrix} = \begin{pmatrix}
8 \\
3
\end{pmatrix} * \frac{5}{4} = 70$

$\begin{pmatrix}
8 \\
5
\end{pmatrix} = \begin{pmatrix}
8 \\
4
\end{pmatrix} * \frac{6}{5} = 84$

c) $3! * (\sum_{k = 1}^{10} 10-k)+ 3 = 6 * (9+8+7+6+5+4+3+2+1) + 3 = 273$

$+3$  im Fall dass man 10 als erste Variable nimmt. $*3!$, weil es $3!$ mögliche Permutationen gibt wenn man die erste Variable auf 1-9 setzt. 

---

### Aufgabe 2

a) Induktionsverankerung mit n = 1:

$\frac{1}{2} = 1-\frac{1}{2}$

Induktionsschritt:

Angenommen: $\sum_{k=1}^{n} \frac{1}{k(k+1)} =1-\frac{1}{n+1}$

Es gilt zu Beweisen: $\sum_{k=1}^{n+1}\frac{1}{k(k+1)} = 1- \frac{1}{n+2}$

$\sum_{k=1}^{n} \frac{1}{k(k+1)} =1-\frac{1}{n+1}$  | $+\frac{1}{n+1(n+2)}$

$\sum_{k=1}^{n+1}\frac{1}{k(k+1)} =1-\frac{1}{n+1} +\frac{1}{(n+1)(n+2)}$    |$*\frac{(n+1)(n+2)}{(n+1)(n+2)}$

$\sum_{k=1}^{n+1}\frac{1}{k(k+1)} =1 - \frac{n+2}{(n+1)(n+2)} + \frac{1}{(n+1)(n+2)} = 1+\frac{1-n-2}{(n+1)(n+2)}$

$\sum_{k=1}^{n+1}\frac{1}{k(k+1)} = 1+\frac{-(1+n)}{(n+1)(n+2)}= 1- \frac{1}{n+2}$ qed

b) Induktionsverankerung mit n = 1:

$\begin{pmatrix}
1 \\
k
\end{pmatrix} \leq 1 \leq 2^{0}$ 

Angenommen:

$\begin{pmatrix}
n \\
k
\end{pmatrix} = \frac{n!}{k!(n-k)!}\leq 2^{n-1}$

Es gilt zu Beweisen: $\begin{pmatrix}
n+1 \\
k
\end{pmatrix}  = \frac{n!*(n+1)}{k!(n-k)!*(n-k+1)} \leq 2^n$

$\begin{pmatrix}
n \\
k
\end{pmatrix} = \frac{n!}{k!(n-k)!}\leq 2^{n-1}$    | $*2$

$2\begin{pmatrix}
n \\
k
\end{pmatrix} = \frac{2n!}{k!(n-k)!}\leq 2^{n}$

Es gilt zu beweisen: $\frac{n!*(n+1)}{k!(n-k)!*(n-k+1)} ≤ \frac{2n!}{k!(n-k)!}$

also $\frac{n+1}{n+1-k}≤ 2$      $\forall n,k \in \mathbb{N}, k≤n$

Induktionsverankerung mit n = 1:

$\frac{1+1}{1+1-k}≤ 2$            $\forall k \in \mathbb{N}$

Induktionsschritt:

c) Induktionsverankerung mit n = 0:

$\sum_{m = k}^{0}\begin{pmatrix}
m \\
k
\end{pmatrix} = 0= \begin{pmatrix}
1 \\
k+1
\end{pmatrix}$

Es gilt zu beweisen: $\sum_{m = k}^{n+1}\begin{pmatrix}
m \\
k
\end{pmatrix} = \begin{pmatrix}
n+2 \\
k+1
\end{pmatrix} = \frac{(n+2)!}{k!(n+2-k)!}$

$\sum_{m = k}^{n}\begin{pmatrix}
m \\
k
\end{pmatrix} = \begin{pmatrix}
n+1 \\
k+1
\end{pmatrix} = \frac{n!}{k!(n-k)!}$           |$+ \begin{pmatrix}
n+1 \\
k
\end{pmatrix}$ 

$\sum_{m = k}^{n+1}\begin{pmatrix}
m \\
k
\end{pmatrix} = \begin{pmatrix}
n+1 \\
k+1
\end{pmatrix} + \begin{pmatrix}
n+1 \\
k
\end{pmatrix} = \frac{n!}{k!(n-k)!} + \frac{(n+1)!}{k!(n+1-k)!}$

$\sum_{m = k}^{n+1}\begin{pmatrix}
m \\
k
\end{pmatrix} = \begin{pmatrix}
n+1 \\
k+1
\end{pmatrix} + \begin{pmatrix}
n+1 \\
k
\end{pmatrix}  = \begin{pmatrix}
n+2 \\
k+1
\end{pmatrix}$ (Rekursionsformel) qed

---

### Aufgabe 3

a)

$e = 7,  n = 3$

$7 - \frac{3f}{2} + f = 2$     , daraus folgt:

$f = 10$

$k = \frac{3f}{2} = \frac{3*10}{2} = 15$

b) 

![[Untitled]]

![[Untitled]]