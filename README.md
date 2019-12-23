\documentclass{article}
\usepackage[utf8]{inputenc}
\usepackage{lipsum,multicol,amsmath}

\title{Linear Regression}
\author{Arief Rahman Fajri 18523092 \\ Faiq Dhimas Wicaksono 18523088}
\date{December 2019}

\begin{document}
\maketitle
\paragraph{Linear Regression}
\begin{align*}
\begin{tabular}{|c|c|c|c|c|c|}
\hline
$x_{i}$ & $y_{i}$ & $xy$ & $x_{i}^2$ & $y'$ & $(y_{i}-y'_{i})^2$   \\
\hline
$$ 1     & -1.4   & -1.4     & 1        &-0,2490        &1,3248$$\\
$$ 2     & -3.3   & -6.6     & 4        &-3,0315        &0,0720$$ \\
$$ 3     & -6.2   & -18.6    & 9        &-5,8139        &0,1490$$\\
$$ 4     & -7.3   & -29.2    & 16       &-8,5963        &1,6803$$ \\
$$ 5     & -11.1  & -55.5    & 25       &-11,3787       &0,0776$$\\
$$ 6     & -12.3  & -73.8    & 36       &-14,1612       &3,4640$$ \\
$$ 7     & -16.8  & -117.6   & 49       &-16,9436       &0,0206$$ \\
$$ 8     & -20.2  & -161.6   & 64       &-19,7260       &0,2246$$ \\
$$ 9     & -23.4  & -210.6   & 81       &-22,5084       &0,7949$$ \\
$$ 10    & -25.7  & -257     & 100      &-25,2909       &0,1673$$ \\
\hline
\end{tabular}
\end{align*}
\begin{align*}
    a = \frac{n.\sum_{i=1}^{n}x_{i}y_{i} - \sum_{i=1}^{n}x_{i} . \sum_{i=1}^{n}y_{i}}{n.\sum_{i=1}^{n}x_{i}^2 - \left(\sum_{i=1}^{n}x_{i}\right)^2}
\end{align*}
\begin{align*}
    b = \frac{1}{n}\left(\sum_{i=1}^{n}y_{i} - a . \sum_{i=1}^{n}x_{i} \right)
\end{align*}
\paragraph{Answers:}
\begin{enumerate}
    \item 
        \begin{align*}
            a &= \frac{10(-931,9) - 55(-127,7)}{10(385) - 55^2}\\
            &= \frac{-9319 + 7023,5}{3850 - 3025}\\
            &= \frac{-2295,5}{825}\\
            &= -\frac{91,82}{33}
        \end{align*}
        \begin{align*}
            b &= \frac{1}{10}\left(-127,7 -  \left(-\frac{91,82}{33} . 55\right) \right)\\
            &= \frac{1}{10} \left(\frac{-4214,1}{33} - \left(-\frac{5050,1}{33}\right)\right)\\
            &= \frac{1}{10}\left(\frac{836}{33}\right)\\
            &= \frac{836}{330}\\
            &= \frac{83,6}{33}
        \end{align*}
     \begin{align*}
         y &= ax + b\\
         y &= -\frac{91,82}{33}x + \frac{83,6}{33}
     \end{align*}
     
     \item
        \begin{align*}
            E = f &= \sum_{i}^{m}(y_{i}-y'{i})^2\\
            &= 1,3248+0,0720+0,1490+1,6803+0,0776+3,4640\\
            &+ 0,0206+0,2246+0,7949+0,1673\\
            &= 7,9751
        \end{align*}
        
\end{enumerate}
\end{document}

