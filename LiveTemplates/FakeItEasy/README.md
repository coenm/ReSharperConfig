# FakeItEasy

Typing `mhh1` (Must Have Happened 1 time) inside a test method will expand to:

```csharp
FakeItEasy.A.CallTo(() => $methodCall$).MustHaveHappenedOnceExactly();$END$
```

Typing `mnhh` (Must Not Have Happened) inside a test method will expand to:

```csharp
FakeItEasy.A.CallTo(() => $methodCall$).MustNotHaveHappened();$END$
```
