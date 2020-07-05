FROM ubuntu:18.04

RUN apt-get update && apt-get install -y \
    git make wget \
    xdvik-ja \
    evince \
    cpanminus \
    language-pack-ja \
    xzdec \
    latexmk \
    texlive-lang-cjk \
    texlive-latex-extra \
    texlive-extra-utils \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN tlmgr init-usertree
RUN kanji-config-updmap-sys ipaex
