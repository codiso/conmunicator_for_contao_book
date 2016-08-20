# Mehrsprachigkeit

Adobe Muse CC unterstützt von Hause aus keine mehrsprachigen Seiten. In Contao ist die Realisierung der Mehrsprachigkeit eine relativ leicht zu lösende Aufgabe.

Die Frage stellt sich nun, wie geht man in diesem speziellen Fall mit den Stilen in Adobe Muse CC um. Es muss für die entsprechenden Inhalte eine Sprachangabe gemacht werden.

So lange man Layoutbereiche nutzt, werden Inhalte automatisch immer aus der jeweiligen Sprachversion genommen und dargestellt. Dies gilt auch für eigene Layoutbereiche \(Sections\).

Weist man aber beispielsweise Artikel, Inhaltselemente oder Module zu, so besitzt der Stil immer auch eine Angabe der Zielsprache.

```
cmu_article_de_23
```

In diesem Falle würde der Artikel mit der ID 23 in der deutschen Sprache genutzt.

```
cmu_article_de_23 | cmu_content_en_45
```

Durch die Angabe eines kombinierten Stils in Adobe Muse CC, kann für jede Sprache eine eigene Angabe über den genutzten Inhalt gemacht werden. Trennen Sie die Angaben durch " \| " oder " - ". Beachten Sie die Leezeichen vor und nach dem Trennzeichen!


