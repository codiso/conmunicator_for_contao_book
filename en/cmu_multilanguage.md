# Multilanguage

Adobe MUSE supports inherently no multilingual sites. In Contao the realization of multilingualism is a relatively easy task to be solved.

Now a question arises how to handle the project in this particular case, with using styles in Adobe-MUSE. The solution is to define the language information in the specific style.

As long as you use layout sections, contents are always taken from the respective language version shown in the layout areas. This also applies to custom layout sections.

```
cmu_article_de_23
```

In this case, the article with ID 23 would be used in the German language.

```
cmu_article_de_23 | cmu_content_en_45
```

By specifying a combined style in Adobe Muse, a separate indication of the shared content can be made for each language. Seperate the styles by " | " or " - ". Be aware of the whitespaces before and after the seperator.

