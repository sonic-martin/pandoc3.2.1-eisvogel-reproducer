# Reproducer

This is a reproducer for [Wandmalfarbe/pandoc-latex-template#391](https://github.com/Wandmalfarbe/pandoc-latex-template/issues/391).

![image](picture.png "Random test image")

## Works with Pandoc 3.2.0

```
docker run --rm -v "`pwd`:/data" pandoc/extra:3.2.0 readme.md -o doc.pdf --template=eisvogel
```

## Works not with Pandoc 3.2.1

```
docker run --rm -v "`pwd`:/data" pandoc/extra:3.2.1 readme.md -o doc.pdf --template=eisvogel
```
