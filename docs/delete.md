<h1 align="center"><u>PysonDB</u></h1>


* [Install](https://github.com/fredysomy/pysonDB)
* [Example Code](https://github.com/fredysomy/pysonDB/example)
* [Command Line Operations](https://markdownitweb.herokuapp.com/cli-0e4d)
* [Adding Data](https://markdownitweb.herokuapp.com/add_data-c37f)
* [Get data](http://markdownitweb.herokuapp.com/getdata-fd3b)
* [Update Data](https://markdownitweb.herokuapp.com/updatedata-fd97)
* [Delete Data](https://markdownitweb.herokuapp.com/deletedata-6ead)

<h2>Delete Data</h2>

* Methods
  * deleteById(ID)
  * Deletes the JSON data with the given ID 

***

>>JSON file:file.json

```json
{"data": [{"name": "PysonDB", "type": "DB", "score": "10", "id": 5161221802},
{"name": "Pyson-CLI", "type": "CLI", "score": "10", "id": 2242313690},
{"name": "Tiny", "type": "DB", "score": "9", "id": 6991190264},
{"name": "QWERTY", "type": "DB", "score": "5", "id": 9416036202}]}
```

***  

<h2><code>deleteById(ID)</code></h2>

```python
>> from pysondb import db
>> a=db.getDb("file.json")
>> a.deleteById("6991190264")
>> # The JSON data with ID "6991190264" is deleted.Lets verify.
>> a.getAll()
>> [{"name": "PysonDB", "type": "DB", "score": "10", "id": 5161221802},
{"name": "Pyson-CLI", "type": "CLI", "score": "10", "id": 2242313690},
{"name": "QWERTY", "type": "DB", "score": "5", "id": 9416036202}]
```

***

* See full examples [here](https://github.com/fredysomy/pysonDB/example).
* If You have any queries or doubts join the discord server [here](https://discord.gg/SZyk2dCgwg)