---
tags:
  - kategoria
---

```dataview
table without id
	file.link as Nazwa,
	ważność as Ważność,
	url as WWW
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort ważność desc
```