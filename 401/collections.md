# Collections & Enum

##  [Collections](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections)

**Collections** are groups of information. 

<a href="/en-us/dotnet/api/system.collections.generic.dictionary-2" data-linktype="absolute-path">Dictionary&lt;TKey,TValue&gt;</a> 
 Represents a collection of key/value pairs that are organized based on the key. 
 

 <a href="/en-us/dotnet/api/system.collections.generic.list-1" data-linktype="absolute-path">List&lt;T&gt;</a> 
 Represents a list of objects that can be accessed by index. Provides methods to search, sort, and modify lists. 
 

 <a href="/en-us/dotnet/api/system.collections.generic.queue-1" data-linktype="absolute-path">Queue&lt;T&gt;</a> 
 Represents a first in, first out (FIFO) collection of objects. 
 

 <a href="/en-us/dotnet/api/system.collections.generic.sortedlist-2" data-linktype="absolute-path">SortedList&lt;TKey,TValue&gt;</a> 
 Represents a collection of key/value pairs that are sorted by key based on the associated <a href="/en-us/dotnet/api/system.collections.generic.icomparer-1" data-linktype="absolute-path">IComparer&lt;T&gt;</a> implementation. 
 

 <a href="/en-us/dotnet/api/system.collections.generic.stack-1" data-linktype="absolute-path">Stack&lt;T&gt;</a> 
 Represents a last in, first out (LIFO) collection of objects. 


## [Enum](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/enum)
>If you want an enumeration type to represent a combination of choices, define enum members for those choices such that an individual choice is a bit field. That is, the associated values of those enum members should be the powers of two. Then, you can use the bitwise logical operators | or & to combine choices or intersect combinations of choices, respectively. To indicate that an enumeration type declares bit fields, apply the Flags attribute to it. As the following example shows, you can also include some typical combinations in the definition of an enumeration type.