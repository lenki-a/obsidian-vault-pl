```dataview
table without id
	file.link as osoba,
	telefon as telefon
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```