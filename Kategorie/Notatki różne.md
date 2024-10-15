```dataview
table without id
	file.link as Nazwa,
	data as Data
where
  contains(kategoria,this.file.link) and
  !contains(file.name,"szablon")
sort file.name asc
```

