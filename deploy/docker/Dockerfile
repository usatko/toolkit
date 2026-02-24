FROM sharelatex/sharelatex:latest

# 1. Update the TeX Live Manager itself
RUN tlmgr update --self


# 2. Install all the specific packages requested in report.tex and report-sl.tex
RUN tlmgr install \
    ucs \
    tabulary \
    fancyhdr \
    xcolor \
    parskip \
    vmargin \
    setspace \
    pgfplots \
    pgf-pie \
    pdflscape \
    smartdiagram \
    xstring \
    multirow \
    shipunov \
    appendix \
    listings \
    lipsum \
    natbib \
    hyperref \
    babel-english \
    babel-slovenian \
    hyphen-slovenian \
    # 3. Rebuild the TeX file database so the compiler sees the new packages
    && texhash
