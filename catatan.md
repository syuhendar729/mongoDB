# Database

## method yg penting aja
```
db.dropDatabase() 		=> menghapus database
db.getName()			=> mengambil nama databse
db.hostInfo()			=> mengambil info host tmpt mongodb
db.version()			=> versi database
db.stats()				=> mengambil statistik penggunaan database
```

# Collection
- Tempat penyimpanan document (seperti table di mysql)
- Max per-document yg bisa disimpan 16Mb
- Max level nested document yg bisa disimpan adalah 100level
## bbrp method yg penting

### method database untuk collection
```
db.getCollectionNames()		=> mengambil semua nama collection
db.createCollection(name)	=> membuat collection baru
db.getCollection(name)		=> mendapatkan object collection
db.<name> 					=> sama dgn db.getCollection(name)
db.getCollectionInfos()		=> mendapat informasi sebuah collection
```

```mongoshell
> use belajar
switched to db belajar
> db.createCollection('contoh')
{ "ok" : 1  }
> show dbs
admin    0.000GB
belajar  0.000GB
config   0.000GB
local    0.000GB
nodejs   0.000GB
> show collections
contoh
> db.getCollectionNames()
[ "contoh"  ]
> db.createCollection('produk')
{ "ok" : 1  }
> db.getCollectionNames()
[ "contoh", "produk"  ]
>
```

### collection method
```
db.<collection>.find() 			=> mengambil semua document
db.<collection>.count()			=> jumlah document
db.<collection>.drop()			=> menghapus collection
db.<collection>.totalSize()		=> mengambil total ukuran collection
db.<collection>.stats()			=> mengambil info statistik collection
```










