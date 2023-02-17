# Cheat Sheet - LaTeX

## Opmaak

- [online help](https://nl.wikibooks.org/wiki/LaTeX/Tekstopmaak)

```LaTeX
{\bf Vette tekst.}
\hline
``Een tekst''     %“Een tekst”
```

- Te lange hyperlinkken

```LaTeX
\usepackage[bookmarks=true,breaklinks]{hyperref}
```

### Code

#### Inline

```LaTeX
directory \verb|C:\Windows\system32|  %directory C:\Windows\system32
het \verb+\ldots+ commando            %het \ldots commando
```

#### Block

- Letterlijke tekst in een block - verbatim

```LaTeX
\begin{verbatim*}
Alle tekst \texttt{verbatim} die hier
staat
wordt in \LaTeX{} letterlijk weergegeven.
\end{verbatim*}
```

- Letterlijke tekst in een block - lstlisting

```LaTeX
\begin{lstlisting}[language=Python]
	%code
\end{lstlisting}
```

- Opmaak

```LaTeX
\documentclass{article}
\usepackage{listings}
\usepackage{xcolor}

\definecolor{codegreen}{rgb}{0,0.6,0}
\definecolor{codegray}{rgb}{0.5,0.5,0.5}
\definecolor{codepurple}{rgb}{0.58,0,0.82}
\definecolor{backcolour}{rgb}{0.95,0.95,0.92}

\lstdefinestyle{mystyle}{
    backgroundcolor=\color{backcolour},   
    commentstyle=\color{codegreen},
    keywordstyle=\color{magenta},
    numberstyle=\tiny\color{codegray},
    stringstyle=\color{codepurple},
    basicstyle=\ttfamily\footnotesize,
    breakatwhitespace=false,         
    breaklines=true,                 
    captionpos=b,                    
    keepspaces=true,                 
    numbers=left,                    
    numbersep=5pt,                  
    showspaces=false,                
    showstringspaces=false,
    showtabs=false,                  
    tabsize=2
}

\lstset{style=mystyle}

\begin{document}
The next code will be directly imported from a file

\lstinputlisting[language=Octave]{BitXorMatrix.m}
\end{document}
```

- minted (extra config nodig .. pip install Pygments)

```LaTeX
\documentclass{article}
\usepackage{minted}
\begin{document}
\begin{minted}{python}
  %code
\end{minted}
\end{document}
```

## Referenties

**Note**: Gebruik de tilde **~** om ongewenste pagina/paragraaf afkappingen te vermijden tijdens het refereren.

## Lijsten

### Gesorteerde / Genummerde lijst - enumerate

```LaTeX
genummerde (gesorteerde) lijsten zijn eenvoudig te maken:
\begin{enumerate}
  \item nummering is automatisch.
  \item nummering start met 1 en gebruikt de \texttt{enumerate} omgeving.
  \item nog een genummerd item in de lijst.
\end{enumerate}
```

### Ongesorteerde / Bullets lijst - itemize

```LaTeX
\begin{itemize}
   \item First level item
   \item First level item
   \begin{itemize}
     \item Second level item
     \item Second level item
     \begin{itemize}
       \item Third level item
       \item Third level item
       \begin{itemize}
         \item Fourth level item
         \item Fourth level item
       \end{itemize}
     \end{itemize}
   \end{itemize}
 \end{itemize}
```

## Afbeelding - fig

**Note**: `\caption` moet voor `\label`

### Opmaak figuur

```LaTeX
%ref in tekst
.. dit kan je bekijken in Figuur ~\ref{fig:refVoorbeeldAfbeelding} op pagina ~\pageref{fig:refVoorbeeldAfbeelding}.


\begin{figure}[h]
    \includegraphics[width=1\textwidth]{img/afbeelding01.png}
    \caption{Voorbeeld van Afbeelding}
    \label{fig:refVoorbeeldAfbeelding}
\end{figure}
```

### Schalen

```LaTeX
\includegraphics[scale=1.5]{overleaf-logo}
\includegraphics[width=5cm, height=4cm]{overleaf-logo}
```

### Voorbeeld

```LaTeX
\begin{figure}
    \centering
    \includegraphics[width=1\linewidth]{img/aanvallen72h.png}
    \caption{Evolutie geregistreerde Log4shell aanvalspogingen door Checkpoint van 11/12/2021 tot 13/12/2021.}
    \label{fig:aanvallen72h}
\end{figure}
```

## Tabel - tab

Tabellen kunnen eenvoudig opgemaakt worden via de [tablegenarator](https://www.tablesgenerator.com/latex_tables) en extra verfraaiingen kan je dan later toevoegen.

### Opmaak tabel

```LaTeX
\begin{table}[t]
    \centering
    \begin{tabular}{}
        %table content
    \end{tabular}
    \caption{}
    \label{tab:label}
\end{table}
```

### Uitgebreid

```LaTeX
%referentie in tekst
.., we kunnen dit afleiden uit de bijhorende tabel~\ref{tab:refVoorbeeldTabel}.

%onderstaande tabel is met de opmaak zoals in de cursus aangeraden wordt
\begin{table}[]
    %label
    \caption[smv-label]{Uitgebreide tekst voor het Label}
    \begin{tabular}{@{}lll@{}}
        \toprule
        \textbf{Hoofding kol1}  & \textbf{Hoofding kol2}    & \textbf{Hoofding kol3}    \\ \midrule
        txt rij2 kol1           & txt rij2 kol2             & txt rij2 kol3             \\
        txt rij3 kol1           & txt rij3 kol2             & txt rij3 kol3             \\
        txt rij4 kol1           & txt rij4 kol2             & txt rij4 kol3             \\
        txt rij5 kol1           & txt rij5 kol2             & txt rij5 kol3             \\ \bottomrule
    \end{tabular}
    %referentie in tekst
    \label{tab:refVoorbeeldTabel}
\end{table}
```

**Note**: opletten met **&**-tekens in tabellen !!
