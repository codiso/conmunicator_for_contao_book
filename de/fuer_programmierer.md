# Für Programmierer …

Betrachtet man die Seite der Gestaltung aus Sicht des Adobe Muse CC Projektes, so sind Stile die einfachste und unkomplizierteste Art dynamische Inhalte aus dem Contao-CMS mit dem statischen Layout zu verbinden.

Bei komplizierteren Ansprüchen, wird man mit Stilen alleine nicht ans Ziel gelangen. Hier benötigt man mehr Kontrolle über die Zuordnung von dynmaischen Inhalten zu den DOM-Elementen des HTML-Dokumentes.

Mit &lt;.CONMUNICATOR&gt; hat man verschiedene Möglichkeiten die Zuordnung zu kontrollieren oder eigenen Code einzubinden.

| Art: | Datei: | Bedeutung: |
| --- | --- | --- |
| Content-Mapping | content\_mapping\_[LANG].php | Inhalte aus Contao können über XPath zugeordnet werden. |
| File-Mapping | file\_mapping.php | Seiten aus Contao können über den Seitenalias manuell Adobe Muse CC Seiten zugeordnet werden. |
| Code at end of head | code\_at\_end\_of\_head.php | Um eigenen Code am Ende des &lt;head&gt; zu plazieren. |
| Code at end of body | code\_at\_end\_of\_body.php | Um eigenen Code am Ende des &lt;body&gt; zu plazieren. |
| Text replacement | text\_replacement.php | Texte finden und durch  ersetzen. |

## Adaptives Layout

Mit Adobe Muse CC kann ein Layout adaptiv aufgebaut werden. Es entstehen, bei einem Export aus Adobe Muse CC, drei unabhängige Sites. Diese werden in entsprechenden Ordnern abgelegt.

| Gerät: | Bedeutung: |
| --- | --- |
| Desktop | Inhalte für die Darstellung auf einem Desktop-Computer oder Laptop, werden auf der obersten Ebene des Exports abgelegt. |
| Tablet | Inhalte für die Darstellung auf einem Tablet befinden sich im Ordner **\/tablet**. |
| Phone | Inhalte für die Darstellung auf einem Tablet befinden sich im Ordner **\/phone**. |

Damit eine Kontrolle der einzelnen Versionen möglich wird, besitzt &lt;.CONMUNICATOR&gt; drei Ordner für die genannten exportierten Sites.

* \/devices\/desktop
* \/devices\/tablet
* \/devices\/phone

In jedem dieser Ordner befinden sich die Dateien, zur Kontrolle, der oben genannten Arten.

## Responsives Layout

In aktuellen Version von Adobe Muse CC können Layouts responsiv aufgebaut werden. Hierbei gibt es nur ein Design. Über CSS-Media-Queries wird festlegt wie die Site auf unterschiedlichen Endgeräten visuell aufgebaut wird.

In diesem Falle kann nur der Ordner **\/desktop** für die Kontrolle genutzt werden.

