## Lambda expression And Expression body definition

#### Lambda Declaration Operator:   = > 
*in lambda expression we have a left side and right side*
 
```diff
> A. Expression Bodied Members
```

   **using with:**
+ Constructor
+ Destructor
+ Methods
+ Property, Indexer set accessor
+ void
```diff
- syntax:
> member => expression
```


```c#
// Example:

class Human
{
    // No Returned type (Constructor, Destructor, void)
    
    public Human()=> Console.WriteLine("Hello, World");

    public int x=1;
    public int y =2;
    public Human()=> y=y+x;

    ~Human() => Console.WriteLine("The finalizer is executing.");

}
```   
```diff
> B. lambda expressions 
```

##### *We use it to create an anonymous function*
```diff
- syntax:
> (input-parameters) => expression
> (input-parameters) => { <sequence-of-statements> }
```

 ```c#
// Example:

Func<int,bool> ex = x => x % 2=0;
//Action with sequence-of-statements
 ```
`

`
> Note : Any lambda expression can be converted to a delegate type
