###CREATE a table called 'receipts' that has the following columns: id, store, item, number_of_items, price, and buy_date.

```sqlite> CREATE TABLE receipts (id INTEGER PRIMARY KEY AUTOINCREMENT, store TEXT, item TEXT, number_of_items INTEGER, price INTERGER, buy_date DATE); ```

* check to see table record 

```
sqlite> .schema 

CREATE TABLE receipts (id INTEGER PRIMARY KEY AUTOINCREMENT, store TEXT, item TEXT, number_of_items INTEGER, price INTERGER, buy_date DATE);
sqlite> 
```

All the attributes from all the receipts
**sqlite> SELECT * FROM receipts;**
The store and item names from all the receipts
**sqlite> SELECT store,item FROM receipts;**
All the attributes from all purchases made at Toys R Us
**sqlite> SELECT * FROM receipts WHERE store = "Toys R Us";**
The item name of each purchase made at Strand.
**sqlite> SELECT item FROM receipts WHERE store = "Strand";**
The total number of items Peter purchased
**sqlite> SELECT number_of_items FROM receipts;**
The total number of items purchased at Sears
**sqlite> SELECT number_of_items FROM receipts WHERE store = "Sears";**
All the attributes of receipts where Peter bought multiple items.
**sqlite> SELECT * FROM receipts WHERE number_of_items > 1;**
The average number of items purchased on a trip to JC Penny
**sqlite> SELECT avg(number_of_items) FROM receipts WHERE store = "JC Penny";**
Great, now add a new receipt representing the purchase of a single "Heatstreet Maple Bourbon", purchased for $40.99 at "Schnapps Haus" on the most recent fourth of July.
**answer**
