# Example 1: Decimals as Prices

Net Price and Gross Price are both separate (albeit related) concepts within our domain, but because they are both represented by decimals, we lose any concept of type-safety. As far as the type system is concerned, they are interchangeable.

There is nothing stopping us from accidentally passing in a Net price to a method that takes a Gross price.
