# Strings

## String Templates
String templates are done using the following syntax

```csharp
var = 1;
Console.WriteLine($"My cool string with variable {var}");
```

## String Length

String lengths can be discovered using the `Length` property of strings

```csharp
string coolString = "My cool string";
int length = coolString.Length;
```

## String Trimming 
You can trim whitespace before or after a string message by calling `Trim()`, `TrimStart()` , or `TrimEnd()` on a string.

```csharp
string message = "   Hi ";
Console.WriteLine(message.Trim()); //"Hi"
```

## Escape Characters
| Escape Character | Name |
 | ---------------- | ---- |
 | \\'               | Single Quote |
 | \\"               | Double Quote |
 | \\\               | BackSlash    |
 | \0               | Null         |
 | \b               | Backspace    |
 | \n               | New Line     |
 | \t               | Tab          |





## String Replace

Replace parts of strings by using `.Replace(old, new)`

```csharp
string hello = "Hello there";
string goodbye = string.Replace("Hello", "Goodbye"); //Goodbye there
```

## Uppercase/Lowercase

To upper/lowercase a string, use `ToUpper()` or `ToLower()`

```csharp
string hello = "hi";
string string = hello.ToUpper() //HI
```

## Substrings
You can grab a substring of characters from a string by using `.Substring(a, b)` on a string. `a` is the position to start from and `b` is how many charaters to grab. It returns a new string.

```csharp
string a = "I have hte high ground";
SystemConsole.WriteLine(a.Substring(7,2));
```

## Searching Strings

To search strings, use `Contains()`

```csharp
string string = "Hello from the other side";
bool contains = string.Contains("other");
```

### Search Start and End of String
You can also use `StartsWith(s)` and `EndsWith(s)` to find something that starts or ends with a substring `s`

### Find index of specific character

To find a character at a specific location, use `.IndexOf(s)`, where `s` is the messsage. `IndexOf()` will find the first instance. Returns -1 when not found.

```chsarp
int index = string.IndexOf("o");
```

## Null or Empty Strings

```csharp
string s = String.Empty;
String.IsEmptyOrNull(s); // True
```

## Accessing Individual Characters
Strings can be indexed like arrays
```csharp
string message = "A cool hat";
character a = message[0];
```


## String Builder
You can create a `StringBuilder` object to manipulate strings in a different way if you prefer. To get the message stored in the `StringBuilder`, you would call `ToString()`

```csharp
System.Text.StringBuilder sb = new System.Text.StringBuilder("Rat: the ideal pet");
sb[0] = 'C';
System.Console.WriteLine(sb.ToString()); //Cat: the ideal pet
```