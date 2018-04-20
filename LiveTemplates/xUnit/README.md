# xUnit templates

Typing `fact` inside a class will expand to:

```csharp
[Xunit.Fact]
public void $testName$Test()
{
    // arrange
	$END$

    // act

    // assert
}
```

and `afact` is the async variant: 

```csharp
[Xunit.Fact]
public async Task $testName$Test()
{
    // arrange
    $END$

    // act

    // assert
}
```

My test methods are suffixed with 'Test' and follow the arrange-act-assert structure.