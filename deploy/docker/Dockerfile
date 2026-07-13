FROM sharelatex/sharelatex:6.1.2

# 1. Point tlmgr to the frozen 2025 historic repository using an HTTPS mirror
RUN tlmgr option repository https://ftp.math.utah.edu/pub/tex/historic/systems/texlive/2025/tlnet-final

# (Note: We removed 'RUN tlmgr update --self' because a frozen repo has no updates)

# 2. Install all the specific packages requested, including pdfcomment
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
    xkeyval \
    datetime2 \
    zref \
    marginnote \
    soulpos \
    pdfcomment \
    bigfoot \
    acronym \
    pgfgantt \
    # 3. Rebuild the TeX file database
    && texhash
