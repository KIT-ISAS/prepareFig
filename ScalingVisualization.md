Matlab code used to generate the example:
```
close all
plot(1:10,1:10,1:10,2:11)
legend('a','b');
prepareFig([7,7],scaling=1)
exportgraphics(gcf,'Scale1.pdf')

plot(1:10,1:10,1:10,2:11)
legend('a','b');
prepareFig([7,7],scaling=2)
exportgraphics(gcf,'Scale2.pdf')
```
LaTeX code:
```
\documentclass[english]{article}
\usepackage[T1]{fontenc}
\usepackage[latin9]{inputenc}
\usepackage{graphicx}
\usepackage{babel}
\begin{document}
\begin{figure}
\includegraphics{Scale1}

\caption{Scale by 1}
\end{figure}
\begin{figure}
\includegraphics[scale=0.5]{Scale2}

\caption{Scale by 2}
\end{figure}

\end{document}
```