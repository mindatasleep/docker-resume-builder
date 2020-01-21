# Docker + XeTeX Resume Builder

This is a one-page, two asymmetric column resume builder which implements the [moss/xelatex Docker image](https://hub.docker.com/r/moss/xelatex) to compile XeLaTex document and deploy a generated PDF file. The typography and design are inspired by the [https://github.com/deedy/Deedy-Resume](Deedy) design.

## File to edit
```
src/cv_12.tex
```

## Execute locally with XeTeX
```
cd src/
bash run.sh
```

## Spin up Docker build
```
cd src/

# Simple make
docker run --rm -v $PWD:/data moss/xelatex make
# Auto-compile for each save
docker run --rm -v $PWD:/data moss/xelatex make view
```