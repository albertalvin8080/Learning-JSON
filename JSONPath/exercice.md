https://jsonpath.com/

## 1. First element in array:

```ruby
 $.store.book[0]
```

## 2. Array elements from start index up-to index 2 (inclusive):

```ruby
 $.store.book[0:3]
```

## 3. Select first n(2) elements of an array:

```ruby
$.store.book[:2]
```

## 4. Select last n(2) elements of an array:

```ruby
$.store.book[-2:]
```

## 5. Select multiple elements of an array:

```ruby
$.store.book[0,1,3]
```

## 6. Select the elements of an array where price <= 9.00:

```ruby
$.store.book[?(@.price <= 9.00)]
```

## 7. Select the authors of the first two books:

```ruby
$.store.book[:2].author
```

## 8. Select the authors of the last two books:

```ruby
$.store.book[-2:].author
```

## 9. Select the prices of all elements in the store:

```ruby
$.store..price
```

## 10. Select all collections inside the store:

```ruby
$.store.*
```

## 11. Select all books alternating by n(2):

```ruby
$.store.book[::2]
```

## 12. Select all books alternating by n(2) starting from the second book:

```ruby
$.store.book[-1::2]
```

## 13. Select all books which have a price higher than 9 or in which the author is Nigel Rees:

```ruby
$.store.book[?(@.price > 9 || @.author == 'Nigel Rees')]
```

## 14. Select all books which have a price higher than 11 and in which the title is "Sword of Honour":

```ruby
$.store.book[?(@.price > 11 && @.title== 'Sword of Honour')]
```
