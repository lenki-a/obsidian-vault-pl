---
tags: kategoria
---
```dataview
table without id
	file.link as Instrument,
	ticker as Symbol,
	url as URL
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```