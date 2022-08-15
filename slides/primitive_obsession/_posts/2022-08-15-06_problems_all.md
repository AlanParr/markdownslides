# Example 3: All issues together

This scenario is made trickier because ints are implicitly convertible to decimals so there is nothing stopping us from doing this:

```csharp
var brandId = 12;
var productId = 1000;
UpdateProductGrossPrice(productId, brandId, brandId);
```

So using primitives in our above code introduces the following problems:
* The Id for Brands and Products are interchangeable, but in our domain they are not.
* Gross and Net Prices are interchangeable, but in our domain they are not.
* Brand and Product Ids are interchangeable with Gross or Net Price, which they most definitely are not in our domain.
