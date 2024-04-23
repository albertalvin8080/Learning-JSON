https://jsonpath.com/

## 1. First element in array:
 $.store.book[0]

## 2. Array elements from start index up-to index 2 (inclusive):
 $.store.book[0:3]

## 3. Select first n(2) elements of an array:
 $.store.book[:2]

## 4. Select last n(2) elements of an array:
 $.store.book[-2:]

## 5. Select multiple elements of an array:
 $.store.book[0,1,3]

## 6. Select elements of an array where price <= 9.00:
 $.store.book[?(@.price <= 9.00)]

## 7. Select the authors of the first two books:
 $.store.book[:2].author

## 8. Select the authors of the last two books:
 $.store.book[-2:].author

## 9. Select the prices of all elements in the store:
 $.store..price

## 10. Select all collections inside the store:
 $.store.*

## 11. Select the books alternating by n(2):
 $.store.book[::2]

## 12. Select the books alternating by n(2) starting from the second book:
 $.store.book[-1::2]