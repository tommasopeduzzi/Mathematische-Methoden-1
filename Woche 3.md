# Woche 3
![[skriptMMI3.pdf]]
### 2.1 Folgen und Grenzwerte

Bsp.: 2, 4, 6, 8, ...  $a_n = 2n$

1, 4, 9, 16, ...    $a_n = n^2$

1, -1/2, 1/4, -1/8, ... $a_n = (-1)^n\frac{1}{2^n}$

1, 1, 2, 3, 5, 8 ... $a_{n+2} = a_{n} + a_{n+1}$

**Definition 2.1.2:** 

Man nennt eine Folge $**(a_n) n \in \mathbb{N}$** "Nullfolge" (oder sie konvergiert gegen Null):

Zu jedem $\mathbb{e} > 0$  gibt es ein $n_0 \in \mathbb{N}$ . mit $|a_n| < \epsilon$     $\forall n \geq n_0$.

Das bedeutet: Für jeden Epsilon-Streifen gilt: Höchstens  endliche viele Punkte liegen nicht im Epsilon-Streifen.

**Beispiel:**

Siehe Skript

$a_n = \frac{n*3^n}{n!} = \frac{n* 3 * 3* 3 .... * 3}{n*(n-1)*(n-2) * ... * 1}$   $n \in \mathbb{N}$ ist eine Nullfolge.

Bew.: $n^2 * 3^n < 81 * n!$ für n ≥4, durch vollständige Induktion. Daraus folgt (*n! /n) : 

$\frac{n * 3^n}{n!} = 81 * \frac{1}{n}$

zu epsilon > 0 gilt: $a_n < 81/n < \epsilon <=> n > \frac{1}{81\epsilon}$ für alle n ab einem genügend grossen $n_0$

**Definiton 2.1.5: Man sagt, die Folge konvergiert gegen a, wenn  $a_n-a$  eine Nullfolge bildet: Zu jedem $\epsilon > 0$ gibt es ein $n_0$ mit $|a_n -a | < \epsilon$. $\forall n ≥ n_0$**

Beispiele:

1) $a_n = \frac{1-n}{n} = \frac{1}{n} - \frac{n}{n} = \frac{1}{n} -1$

Daher: $\lim_{n -> \infty} a_n = -1$

**Satz 2.1.10: Der Grenzwert einer konvergent Folge $a_n$  ist eindeutig bestimmt,**

**Beweis:** Ang. es gäbe zwei Grenzwerte a<b. Wähle $\epsilon > 0$ so, dass:

 $a + \epsilon < b -\epsilon$ 

$2\epsilon < b-a$

dann wähle $\epsilon < \frac{b-a}{2}$ also z.B. $\epsilon = \frac{b-a}{4}$

Weil Definition: $|a_n -a| < \epsilon$

$-\epsilon < a_n -a < \epsilon$.  | +a

⇒ $a_n < a + \epsilon < b-\epsilon < a_n$ Widerspruch

### Grenzwertrechenregeln:

**Satz 2.1.11:** Ang. $\lim_{n\to\infty} a_n = a$ und $\lim_{n\to\infty} b_n = b$

Dann: $\lim_{n\to\infty} (a_n + b_n) = a+b$

$\lim_{n\to\infty} (a_n * b_n) = a*b$

$\lim_{n\to\infty} \frac{a_n}{ b_n} = \frac{a}{b}$, falls $n \neq 0$

**Konvergenzkriterium 2.1.17:**
Jede monoton steigende Folge (d.h. $a_{n+1}≥ a_n$) die nach oben beschränkt ist (d.h. $a_n ≤ M$ für eine passend Schranke M) hat einen Grenzwert in $\mathbb{R}$.
**Beispiel:** $0.12121212 = \sum_{k=1}^\infty = 12 \sum_{k=1}^\infty (\frac{1}{100})^k = 12 *(\frac{1}{99/100}-1) = \frac{12}{99}$

**Bemerkung 2.1.17**
Beispiel für konvergierende Reihe:
$\sum_{k=1}{\infty}\frac{1}{k^2} = 1 + \frac{1}{4}+ \frac{1}{9}...$

Teilsummenfolge wieder monoton steigend. 
$\sum_{k=1}^{n}\frac{1}{k^2} = 1 + \sum_{k=2}^{n}\frac{1}{k^2} ≤ 1+ \sum_{k=2}^{n}\frac{1}{k*(k-1)} = \sum_{k=1}^{n}\frac{1}{(k+1)*k} = 2- \frac{1}{n}$
Daher $s_n < 2$

Beispiel für divergierende Reihe:
$\sum_{k=1}{\infty}\frac{1}{k} = 1 + \frac{1}{2}+ \frac{1}{3}...$
$\sum_{k=1}{\infty}\frac{1}{k^2} = 1 + \frac{1}{2}+ (\frac{1}{3}+\frac{1}{4}) +(\frac{1}{5}...\frac{1}{8})...$
Die einzelnen Packete lassen sich als $\frac{1}{2}$ abschätzen.

**Beispiel 2.1.19**
$a_{n+1} = \sqrt{2 + a_n}$
a_n ist monoton steigend und nach oben durch $2$ beschränkt.

$a_{n+1} ≥ a_n$       $\forall n$ 
und $a >2$
Beweis durch Induktion n= 1: $a_1 = \sqrt{2} < 2$
$a_2 = \sqrt{a+\sqrt2} > \sqrt{2}$
Induktionsvoraussetzung $n \to n+1$
$a_{n+1} = \sqrt{2+a_n} ≥ a_n$     |$+2$
$a_{n+1} +2 = 2+\sqrt{2+a_n} ≥2+ a_n$
$a_{n+2} )=\sqrt{2+\sqrt{2+a_n}} ≥ a_{n+1}$ qed

$a_n ≤ 2$    |+2
$a_n+2 ≤ 4$ |sqrt
$a_{n+1}  = \sqrt{2+a_n} ≤ 2$ wie behauptet für n +1
Daraus folgt: Grenzwert existiert
Wende Rekursionsformel an:
$a_{n+1} = \sqrt{2+a_n}$  |^2
$a_{n+1}^2 =2+a_n$ 
$\lim_{n\to\infty} a_{n+1}^2 =2+ \lim_{n\to\infty} a_n$ 
$a^2 = 2+a$
Lösung quadratische Gleichung a = 2 oder a=-1 und weil $\sqrt2≤a_n < 2$ und -1 unmöglich ist der Grenzwert 2.

[[Aufgabenblatt 4]]