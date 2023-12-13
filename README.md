- 👋 Hi, I’m @M2j54
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
using System;

class MainClass {
 public static void Main (string[] args) {
    Random random = new Random();
    int n = random.Next(int.MinValue, int.MaxValue);
    Console.WriteLine("The number is: " + n);

    if (n > 0) {
      Console.WriteLine("The number is positive.");
    } else if (n < 0) {
      Console.WriteLine("The number is negative.");
    } else {
      Console.WriteLine("The number is zero.");
    }

    int lastDigit = Math.Abs(n % 10);
    Console.WriteLine("The last digit of the number is: " + lastDigit);

    int a = 5;
    int b = 10;

    Console.WriteLine("Before swapping: a = " + a + ", b = " + b);

    Swap(ref a, ref b);

    Console.WriteLine("After swapping: a = " + a + ", b = " + b);

    PrintLine("Hello, World!");

    PrintReverse("Hello, World!");

    string message = "Hello, World!";
    char prefix = 'H';

    int prefixLength = GetPrefixLength(message, prefix);
    Console.WriteLine("The length of the prefix substring is: " + prefixLength);
 }

 public static void Swap(ref int a, ref int b) {
    int temp = a;
    a = b;
    b = temp;
 }

 public static void PrintLine(string message) {
    Console.WriteLine(message);
 }

 public static void PrintReverse(string message) {
    char[] charArray = message.ToCharArray();
    Array.Reverse(charArray);
    string reversedMessage = new string(charArray);
    Console.WriteLine(reversedMessage);
 }

 public static int GetPrefixLength(string message, char prefix) {
    int prefixLength = 0;
    foreach (char c in message) {
      if (c == prefix) {
        prefixLength++;
      } else {
        break;
      }
    }
    return prefixLength;
 }
}
<!---
M2j54/M2j54 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
