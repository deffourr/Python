# PySpark
Выполнить distinct можно несколькими способами: 
```python
df.distinct().show()
+---+------+---+
| id|  name|age|
+---+------+---+
|  1|Andrew| 26|
|  2| Maria| 30|
|  1|Andrew| 25|
+---+------+---+

df.select(['id', 'name']).distinct().show()
+---+------+
| id|  name|
+---+------+
|  2| Maria|
|  1|Andrew|
+---+------+
###############################################
df.dropDuplicates().show()
+---+------+---+
| id|  name|age|
+---+------+---+
|  1|Andrew| 26|
|  2| Maria| 30|
|  1|Andrew| 25|
+---+------+---+

df.dropDuplicates(['id', 'name']).show()
+---+------+---+
| id|  name|age|
+---+------+---+
|  2| Maria| 30|
|  1|Andrew| 25|
+---+------+---+
```

