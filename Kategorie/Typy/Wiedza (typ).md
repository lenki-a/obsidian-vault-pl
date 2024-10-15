
```dataview
table without id
	file.link as Nazwa,
	data as Data,
	tags as Tagi
where
  contains(typ,this.file.link) and
  !contains(file.name,"szablon")
  sort file.name asc
```