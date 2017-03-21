# Supermarket problem

World’s Groceries Ltd. has prompted us to open a supermarket. At this moment they sell these products:

Product Code | Name | Price
--- | --- | ---
1001 | Tortilla | £ 2.49 
2001 | Sushi | £ 4.99
3001 | Paella | £ 3.45

Initially they want to set these offers to the customers:

* Buy two get one for free (only for Tortillas).
* Buy more than 3 Sushis and the price will drop to £ 4.00.
* Spend more than £ 20.00 and get a free Paella.


## The interface of the software should look like this

```
checkout = new Checkout( princing_rules )
checkout.scan( item1 )
checkout.scan( item2 )

Price = checkout.total
```

Check-out can scan items in any order.


## Some test data

```
Basket: 1001 x 3, 2001 x 1, 3001 x 1
Total: £ 13.42
```

```
Basket: 1001 x 1, 2001 x 10, 3001 x 1
Total: £ 42.49
```