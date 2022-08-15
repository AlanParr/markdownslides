# Solution 1: Decimals as Prices

We can create a simple object to represent our types of price

```csharp
public record GrossPrice(int Value);
public record NetPrice(int Value);
```

Now the type system protects us from sending in the wrong type of price:

```csharp
public void SetGrossPrice(GrossPrice grossPrice) // Can't put a NetPrice here.
{
    // Do something here.
}
```