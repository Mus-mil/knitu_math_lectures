# Неопределённый интеграл

Определение

Неопределённый интеграл функции — это семейство всех  
её первообразных, записываемое в виде:

где:

— первообразная функции, то есть такая функция, что;

— произвольная константа интегрирования.  

---
## Свойства неопределённого интеграла

1️⃣Линейность интеграла  

```math
∫(af(x)+bg(x))dx=a∫f(x)dx+b∫g(x)dx
```

➡️ Это свойство означает, что если функция состоит из  
суммы (или разности) двух функций, умноженных на константы,  
то интеграл можно вычислять отдельно для каждой функции,  
а константы вынести за знак интеграла.  

2️⃣ Интеграл от нуля  
```math
∫0dx=C
```
➡️ Интеграл от нулевой функции всегда равен просто  
произвольной константе CC. Это логично, так как производная  
константы равна нулю, а интеграл — это обратная операция  
к дифференцированию.  

3️⃣ Интеграл от константы  
```math
   ∫adx=ax+C
```
➡️ Если мы берём интеграл от константы, то его результатом  
будет эта же константа, умноженная на переменную xx, плюс  
константа интегрирования.  

4️⃣ Интеграл суммы/разности функций
```math
   ∫(f(x)±g(x))dx=∫f(x)dx±∫g(x)dx
```
➡️ Если у нас есть сумма или разность двух функций, то  
интеграл можно вычислять отдельно для каждой из них,  
а знак ++ или −− просто сохраняется.  

5️⃣ Интеграл от производной
```math
   ∫F′(x)dx=F(x)+C
```
➡️ Если мы берём интеграл от производной функции F′(x)F′(x),  
то мы просто восстанавливаем саму функцию F(x)F(x), так как  
интегрирование и дифференцирование — это обратные операции.  

---

Вычисление неопределённого интеграла в Python

Для нахождения интегралов можно использовать библиотеку sympy:
``` python
import sympy as sp

# Определяем переменную
x = sp.Symbol('x')

# Задаём функцию
f = 3*x**2

# Вычисляем интеграл
integral_f = sp.integrate(f, x)

print(f"∫ 3x² dx = {integral_f} + C")
```
Вывод:
```
∫ 3x² dx = x**3 + C
```