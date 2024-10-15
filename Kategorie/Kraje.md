```dataview
table without id
	file.link as Nazwa,
	kontynent as Kontynent,
	ludność as Ludność
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```