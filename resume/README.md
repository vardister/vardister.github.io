# Resume (LaTeX)

This directory contains the editable LaTeX source for the resume.

## Local setup

Install LaTeX tooling (`texlive` + `latexmk`):

```bash
sudo apt-get update
sudo apt-get install -y latexmk texlive-latex-base texlive-latex-recommended texlive-fonts-recommended texlive-latex-extra lmodern
```

## Build

From the repository root:

```bash
make -C resume build
```

To compile and update the website PDF (`/files/resume_industry.pdf`):

```bash
make -C resume copy
```
