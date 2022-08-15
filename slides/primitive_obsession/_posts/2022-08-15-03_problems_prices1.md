# Example 1: Decimals as Prices

```csharp
public void SetPrice(decimal price)
{
    // Do stuff here.
}
```

What price is this method expecting? We could solve this by just making the name more descriptive right?

```csharp
public void SetGrossPrice(decimal grossPrice)
{
    // Do something here.
}
```

This is better, until we look at how we call it.

```csharp
public void DoSomething()
{
    var grossPrice = 10m;
    var netPrice = 8m;
    
    SetGrossPrice(netPrice);
}
```