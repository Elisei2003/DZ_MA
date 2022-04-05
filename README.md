# DZ_MA

\documentclass{article}
\usepackage[russian]{babel}
\usepackage[utf8]{inputenc}
\usepackage{syntonly}%проверка на ошибки без печати

\title{Интеграл по замкнутому контуру}
\author{Яблонский Елисей}
\date{01.04.2022}

\begin{document}

\maketitle
\begin{thebibliography}{1}
\bibitem{integral}
А.В.Пантелеев, А.С.Акимова. Теория функций комплексного переменного
и операционное исчисление в примерах и задачах

\end{thebibliography}
\section{Задача}

Вычислить интеграл по замкнутому контуру

$\oint_C \frac{e^z}{(z-i)^2(z+2)}dz$

в следующих случаях задания контура а) |z-i|= 2 б) |z+2-i|=3

\section{Решение}

а) В кругу |z-i|<2 присутствует точка z = i. Записываем
функцию 
$\frac{\frac{e^z}{z+2}}{(z-i)^2}$.

И так как в области присутствует один кратный корень то при m = 2 и a = i мы получаем

\par \noindent$\oint_C \frac{e^z}{(z-i)^2(z+2)}dz$ = 2\pi i(\frac{e^z}{z+2})^\prime\bigg|_^z=i
\par\noindentчто равно 2\pi i(\frac{e^z(z+2)-e^z}{(z+2)^2})|_^z=i
\par\noindent= $\frac{2\pi i(i+1)}{(i+2)^2}e^i$
\par\noindentб) в круг |z+2-i|<3 входят две точки i и -2. Расписываем интеграл как сумму двух инетгралов:  \oint_C f(z)dz = \oint_A f(z)dz+\oint_B f(z)dz
\par\noindent где контуры A и B содержат по одной точке. Получаем:
\par\noindent$\oint_C \frac{e^z}{(z-i)^2(z+2)}dz$ = 2\pi i\frac{e^-2}{(2+i)^2}+2\pi i\frac{i+1}{(2+i)^2}e^i = \frac{2\pi i}{(2+i)^2}(e^-2 +(i+1)e^i)

\end{document}
