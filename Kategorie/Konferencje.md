---
tags: kategoria
---
```dataview
table without id
	file.link as Konferencja,
	data as Data,
	url as WWW,
	cena as Cena
where
  contains(konferencja,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```