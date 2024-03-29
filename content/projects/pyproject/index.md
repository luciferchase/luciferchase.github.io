---
title: "PyProject"
date: 2022-01-24
draft: false

type: "posts"
hiddenFromHomePage: false

categories: ["projects"]
tags: ["Coding", "Golang", "Python"]

summary: >-
  Easily kick-start your python project with very opinionated best practices.

featuredImage: screenshot.webp
images: ["screenshot.webp"]
---

# Pyproject

GitHub Repo: [luciferchase/pyproject](https://github.com/luciferchase/pyproject)

Easily kickstart your Python project with very opionionated best practices.

  - [x] Manage your project using poetry <https://python-poetry.org/>
  - [x] Add testing with pytest and pytest-cov
  - [x] Run checks before commiting using pre-commit
  - [x] Code analysis and formatting with Flake8, Mypy, Isort and Black

This is based on this excellant article: [Python Best Practices for a New Project](https://mitelman.engineering/blog/python-best-practice/automating-python-best-practices-for-a-new-project/) and some of my own experiance.

# Installation

{{< admonition type=warning open=true >}}
Poetry must be installed.
{{< /admonition >}}

## `go install`

If you have go installed, simply run:
```bash
go install github.com/luciferchase/pyproject@latest
```

## Binaries

Binaries for Windows are available in the [Release](https://github.com/luciferchase/pyproject/releases) page.\
You have to manually add the `pyproject.exe` file to your path.

## Build from source

`git clone` this repository and run:
```bash
go build -o bin\\pyproject.exe main.go
```
You have to manually add the `pyproject.exe` [availabe in the `.\bin` dir] to your path.

# Why?

Well, dependency management and static typing in Python is a hot mess. To avoid this, we use various tools like `poetry`, `pytest`, `flake8`, `mypy`, `black` and so many more.

Thus to fast track starting a new Python project, I wrote this for myself.
