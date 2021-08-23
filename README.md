# MathParser
C# MathParser


```
//usage
using StringExtensions;

    class Program
    {
        static void Main(string[] args)
        {
            var a="123456+444444 > 0*1000000".ToMath().ToInt();
            Console.WriteLine(a);
            
            var b="$aaa + 100".ToValue(new Dictionary<string, string>(){ {"$aaa", "100"},})
            .ToMath();
            Console.WriteLine(b);

            Console.WriteLine("Hello World!");
        }
    }

```



