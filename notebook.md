# My Coding Notebook
## Table of Contents

-[Flutter Definitions](#flutter_definitions) 
 
  -[Code Definitions](#Code-Definitions)

-[Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)
 
 ## Flutter Definitions

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|   Main()   | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |  | in main dart void main() => runApp(MyPortfolioApp()); |
| MaterialApp     | The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  | main dart return MaterialApp(
  debugShowCheckedModeBanner: false, title: 'TSA Portfolio', and more |
|    Scaffold  | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |  |  return Scaffold( body: Column(mainAxisAlignment: MainAxisAlignment.start,children: [ Padding( padding: const EdgeInsets.only(left: 100.0),child: Column( children: [|
|  colum    | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |  | child: Column( mainAxisAlignment: MainAxisAlignment.center,children: [ |
|     Row | A widget that shows things side-by-side. | `Row(...)` |  |  child: Row( children: [ |
|  Container    | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |  |  return Container( margin: const EdgeInsets.symmetric(vertical: 8, horizontal: 16), padding: const EdgeInsets.all(12), decoration: BoxDecoration( border: Border.all(color: Colors.blue), borderRadius: BorderRadius.circular(12),|
|   Text   | A widget to display text on the screen. | `Text('Hello')` |  |  child: Text(description, style: const TextStyle(color: Colors.white), |
|     Image.network | A widget to show an image using a link from the internet. | `Image.network('https://...')` |  |  child: Image.network('https://placedog.net/640/480?random', fit: BoxFit.cover, |
|    ElevatedButton  | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |  | ElevatedButton( onPressed: () => Navigator.pushNamed(context, '/alt'),child: const Text('Alternate Design'), |
|  onPressed    | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |  |  |
|    StatelessWidget  | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |  |  |
|Navigator| A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |  | Navigator.pushNamed(context, '/alt'),
child: const Text('Alternate Design'), ), |
|   @override   | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  | class MyPortfolioApp extends StatelessWidget {
  @override |
|  build()    | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |  |  |
|   center  | Aligns content in the center of the screen or container. | `Center(child: ...)` |  |  |
|   wrap   | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |  |  |
|   override | This marks a method as one that’s replacing a method in a parent class. | `@override` |  |  |
|  build    | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |  |
|   build   | Required in every widget class to describe what to show. | `build` |  |  |
|    build context  | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |
|    soer key  | A keyword used to pass a value to the parent widget. | `super.key` |  |  |
|   const   | A keyword that means the value won't change and is set once. | `const` |  |  |

 ## Code Definitions
 
 Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|   Variable   | A named container used to store a value that may change. | `var x = 5;` |  | mn dart String title TSA PortFilo |
|  constant    | A fixed value that cannot change once set. | `const PI = 3.14;` |  | mn dart const MyPortFiloApp(superkey) |
|   data type    | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |  |  mn dart bool debugShowCheckedModelBanrner false|
|    String  | A sequence of characters used to represent words or text. | `"Hello World"` |  |  |
|    integer  | Whole number values. | `int age = 16;` |  |  |
|   Double   | Number values with decimals. | `double age = 16.2;` |  |  |
|    Boolean  | A value that can be true or false. | `bool isLoggedIn = false;` |  |  |
|    List  | A collection of values in a specific order. | `List<String> names = [];` |  |  |
|   Null   | A special value that means “nothing.” | `String? name = null;` |  |  |
|    Fuction  | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |  |  |
|  Parameter    | The information passed into a function to change how it works. | `greet(String name)` |  |  |
|    Rturn  | The result a function gives back. | `return total;` |  |  |
|  Scope    | Where a variable or function can be used. | (No set syntax — concept-based) |  |  |
|   Cladd   | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |  |  |
|   Object   | A specific version of a class. | `Dog myDog = Dog();` |  |  |
|   Property   | A variable that belongs to a class/object. | `String name;` |  |  |
|   Methond   | A function that belongs to a class. | `void bark() {}` |  |  |
|   Constructor   | A special function used to set up a class when it’s created. | `Dog(this.name);` |  |  |
|   Abstraction   | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |  |  |
|   Override   | Changing how a built-in or inherited function behaves. | `@override` |  |  |
| Void     | A function that does not return a value. | `void printMessage() {}` |  |  |
| scanner | creates a scanner object to take imput from the user|  |  |  |
|import scanner  |gives acces to scanner class requried at top |  |  |  |
|print line stamnet   |prints the content in the parenthesis adds line after |  |  |  |
|print stamnet   |reads in a string from the user |  |  |  |
| imput nextLine |reads a int from the user |  |  |  |
| imput nextInt |reads a double (decimal) from th user  |  |  |  |
| imput nextDouble | |  |  |  |
|imput nextBoolean  | |  |  |  |
|Aritimetic opretors  | - * / % (noduls retunrs the remainder from dividng  |  |  |  |
| compound operators |applies the result to the variable |  |  |  |
|maximun int  | the max value an int can hold:2147483647 |  |  |  |
| mininum | the minium value an int can hold -2147483647|  |  |  |
|interger overflow  | |  |  |  |
| interger undeflow | |  |  |  |
|round-off error  | |  |  |  |
|overloaded method/function or conctructor   |uses the same name but has a different paramters |  |  |  |
|dot notation |methods are called or objects using a dot after object name |  |  |  |
|concatenate  |to conbime strings with other stringsa and/or varibles   |  |  |  |





































## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
