# Solution 2: Integer Ids

We can create a simple object to represent our IDs

```csharp
public record BrandId(int Value);
public record ProductId(int Value);
```

Now the type system protects us from sending in the wrong id:

```csharp
public void UpdateProductGrossPrice(BrandId brandId, ProductId productId, GrossPrice grossPrice)
{
    // Do something here.
}
```

We can't transpose the Id positions and it is now completely clear what each parameter represents.