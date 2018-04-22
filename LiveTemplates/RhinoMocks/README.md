# RhinoMocks

See [here](https://hibernatingrhinos.com/oss/rhino-mocks) for more information about this framework.

Typing `fake` will create a RhinoMock stub

```csharp
var $var$ = Rhino.Mocks.MockRepository.GenerateStub<$interface$>();$END$
```

Typing `sm` (Stub Method) will expand to

```csharp
$var$.Stub(x => x.$method$).Return($value$);$END$
```

Typing `mhh` (Must Have Happened) inside a test method will expand to:

```csharp
$var$.AssertWasCalled(x => x.$method$);$END$
```

Typing `mnhh` (Must Not Have Happened) inside a test method will expand to:

```csharp
$var$.AssertWasNotCalled(x => x.$method$);$END$
```
