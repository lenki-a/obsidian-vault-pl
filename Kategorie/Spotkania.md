---
tags: kategoria
---
```dataview
table without id
	file.link as Spotkanie,
	data-godzina as Czas,
	osoba as Osoba,
	lokalizacja as Gdzie
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```