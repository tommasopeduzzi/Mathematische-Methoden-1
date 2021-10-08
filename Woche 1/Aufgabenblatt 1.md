# Aufgabenblatt 1

[[Aufgabenblatt 1.pdf]]

# Aufgabenblatt 1

### Frage 1:

d), weil a), b) und c) mögliche Folgerungen aus der Aussage sind.

### Aufgabe 1a:

### Aufgabe 1b:

### Aufgabe 2a:

$\sum_{k=1}^{n} k^2= \frac{n}{6}(n+1)(2n+1)$ $∀n∈ \mathbb{N}$

1. Induktionsverankerung:
    
    n = 1
    
    $1^2 = \frac{1}{6}(1+1)(2+2)$
     ✔️
    
2. Induktionsschritt:
    
    Man nehme an: $\sum_{k=1}^{n} k^2= \frac{n}{6}(n+1)(2n+1)$ 
    
    Zu Beweisen: $\sum_{k=1}^{n+1} k^2= \frac{n+1}{6}((n+1)+1)(2(n+1)+1) = \frac{n+1}{6}(n+2)(2n+3)$ 
    
    $\frac{n+1}{6}(n+2)(2n+3) = \frac{n+1}{6}2n^2 + 7n + 6 = \frac{2n^3 + 9n^2 + 13n+ 6}{6}$
    
     $\sum_{k=1}^{n} k^2= \frac{n}{6}(n+1)(2n+1) | +(n+1)^2$
    
    $\sum_{k=1}^{n+1} k^2= \frac{n}{6}(n+1)(2n+1) +(n+1)^2$
    
    $\sum_{k=1}^{n+1} k^2= \frac{n}{6}(n+1)(2n+1)+n^2 + 2n + 1$
    
    $\sum_{k=1}^{n+1} k^2= \frac{n(n+1)(2n+1)}{6}+\frac{6n^2}{6} + \frac{12n}{6} + \frac{6}{6} = \frac{n(n+1)(2n+1)+6(n+1)^2}{6}$
    
    $\sum_{k=1}^{n+1} k^2= \frac{(2n^3 + 3n^2 + n)+6(n+1)^2}{6} = \frac{(2n^3 + 3n^2 + n)+6(n^2 + 2n + 1)}{6}$
    
    $\sum_{k=1}^{n+1} k^2= \frac{2n^3 + 3n^2 + n +6n^2 + 12n + 6)}{6} = \frac{2n^3 + 9n^2 +13n + 6}{6}$, wie behauptet
    
    ### Aufgabe 2b:
    
    $n! ≥ 2^n$
       $∀n∈\mathbb{N}$ mit $n \geqslant 4$
    
    1. Induktionsverankerung:
        
        $4! = 24 \geq 2^4 = 16$      ✔️
        
    2. Induktionsschritt:
        
        Man nehme an: 
        
        $n! ≥ 2^n$
        
        Zu Beweisen:
        
        $(n+1)! \geq 2^{(n+1)} = 2(2^n)$
        
        $n! \geq 2^n$    | $* (n+1)$
        
        $(n+1)! \geq (n+1)(2^n) > 2(2^n)$, wie behauptet
        
    
    ### Aufgabe 2c:
    
    ### Aufgabe 3a:
    
    Ein Baum ist definiert durch eine Graphen mit mindesten 2 Knoten und keinen Zyklen. Wenn es weniger als zwei Knoten, also einer, hätte, müssten die anderen Punkte einen Zyklus bilden, also wäre es kein Baum. Bei 0 freien Enden ist der ganze Graph ein Zyklus und daher kein Baum.
    
    ### Aufgabe 3b:
    
    Gäbe es mehr als n-1 Kanten, genug um alle n Punkte mit einander zu verbinden, müssten die übrigen Kanten Punkte verbinden, die bereits durch einen Weg verbunden worden sind, würden also einen Zyklus bilden. Es wäre daher kein Baum mehr.