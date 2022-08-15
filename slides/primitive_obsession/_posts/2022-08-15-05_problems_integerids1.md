# Example 2: Integer Ids

The possibility for errors is worse when you consider the below method:
```csharp
public void UpdateProductGrossPrice(int brandId, int productId, decimal grossPrice)
{
    // Do something here.
}
```

```csharp
    UpdateProductGrossPrice(productID, brandID, 12m);
```

Brands and Products are both concepts in our domain and they both have an integer Id which we pass around from method to method, the possibility for swapping these over and creating odd bugs that are potentially quite awkward to find is clear.