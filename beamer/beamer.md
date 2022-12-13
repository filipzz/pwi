# Projekt PWI: Slides generator

## Cel projektu

Napisz program, który konwertuje pliki w formacie [Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) na pliki w formacie [LaTeX Beamer](https://tug.ctan.org/macros/latex/contrib/beamer/doc/beameruserguide.pdf).


Działanie programu ma być analogiczne do działania programu [pandoc](https://pandoc.org/) tj. 

```bash
pandoc notes.md -t latex -o notes.tex
```

z tym, że Twój program ma wspierać opcję tworzenia slajdów ze wskazanym obrazkiem jako pełnowymiarowym tłem (pandoc
umożliwia jedynie ``tradycyjne'' wstawianie obrazów).
