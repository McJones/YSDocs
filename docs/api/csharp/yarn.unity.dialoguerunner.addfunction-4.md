# DialogueRunner.AddFunction(string,System.Func<TResult, T1, T2>)

Method in [DialogueRunner](/docs/api/csharp/yarn.unity.dialoguerunner.md)

## Summary


Add a new function that returns a value, so that it can be
called from Yarn scripts.


```csharp
public void AddFunction<TResult, T1, T2>(string name, System.Func<TResult, T1, T2> implementation);
```

## Remarks

<p>When this function has been registered, it can be called from
your Yarn scripts like so:</p> <pre lang="yarn">
&lt;&lt;if myFunction(1, 2) == true&gt;&gt;
myFunction returned true!
&lt;&lt;endif&gt;&gt;
</pre> <p>The <code>call</code> command can also be used to invoke the function:</p> <pre lang="yarn">
&lt;&lt;call myFunction(1, 2)&gt;&gt;
</pre>

## Parameters

|Name|Description|
|:---|:---|
|`Func<TResult, T1, T2>` implementation|The  <code>System.Delegate</code>  that should be invoked when this function is called.|
|`string` name||

## Type Parameters

|Name|Description|
|:---|:---|
|TResult|The type of the value that the function should return.|
|T1|The type of the first parameter to the function.|
|T2|The type of the second parameter to the function.|

## See Also

* [Library](/docs/api/csharp/yarn.library.md): A collection of functions that can be called from Yarn programs.

