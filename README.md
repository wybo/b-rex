### Beamer Ruby Latex

Beamer-Ruby-Latex, b-rex in short, is a program for pre-parsing latex beamer presentations & papers, and building them with pdflatex and bibtex.

#### Usage

To turn tex file into pdf

    ./b-rex beamer.tex

Other examples:
  
    b-rex -a beamer.tex
    b-rex -e --verbose beamer.tex

#### In Presentations

Instead of:

      \begin{frame}
        \frametitle{My Very Title}
        bigskip

        \begin{itemize}
          \item this point people
          \item do not forget
        \end{itemize}
      \end{frame}

 You can write:
  
      --- My Very Title
  
        * this point people
        * do not forget
  
      ---

It is capable of falling back to normal latex where needed (for the title-page you still use normal latex) and also has support for slides with an image, tables of contents, an intro-frame and higlighted words (by enclosing them in '~''s, ~like this~)

For more info, run with -h opton, and for the latest source code see: https://github.com/wybo/b-rex

#### Requirements

Ruby (inc rdoc, not included in Debian & Ubuntu, needs ruby and rdoc packages there), Latex beamer, and a working TeX Live (the texlive (better texlive-full) and latex-beamer packages are all you need on Ubuntu)

#### Copyright

Copyright (c) 2007-2016 Wybo Wiersma. Licensed under the Affero GPL: http://www.fsf.org/licensing/licenses/agpl-3.0.html
