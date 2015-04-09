###CREATE a table called 'receipts' that has the following columns: id, store, item, number_of_items, price, and buy_date.

```sqlite> CREATE TABLE receipts (id INTEGER PRIMARY KEY AUTOINCREMENT, store TEXT, item TEXT, number_of_items INTEGER, price INTERGER, buy_date DATE); ```

* check to see table record 

```
sqlite> .schema 

CREATE TABLE receipts (id INTEGER PRIMARY KEY AUTOINCREMENT, store TEXT, item TEXT, number_of_items INTEGER, price INTERGER, buy_date DATE);
sqlite> 
```


