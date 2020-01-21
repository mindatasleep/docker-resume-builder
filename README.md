# Docker + XeTeX Resume Builder

This is a one-page, two asymmetric column resume builder which implements the [moss/xelatex Docker image](https://hub.docker.com/r/moss/xelatex) to compile XeTeX into PDF. The design is inspired by the [https://github.com/deedy/Deedy-Resume](Deedy) layout.

## Edit this file
```
src/cv_12.tex
```

## Execute locally with XeTeX
```
cd src
bash run.sh
```

## Spin up Docker build
```
Simple make
docker run --rm -v $(shell pwd):/data moss/xelatex make
Auto compile for each save
docker run --rm -v $(shell pwd):/data moss/xelatex make view
```