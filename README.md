# workspace-cs106-v3

Eclipse workspace used for CS106, CS165, and CS180.  It includes:
*  The JavaCoreTemplate project:  make a copy of this project when starting each assignment.
*  Eclipse preferences set to support easier coding in Java.


# JavaCoreTemplate

Includes:
* `Program.java`, with a `main()` that is ready to go, and has useful classes statically imported.

* `commons-lang3`:  With the wonderful `StringUtils`, which has `join`, `substringsBetween`, `reverse`, etc.  For example:
```java
String[] titles = substringsBetween(quakesXml, "<title>M ", "</title>");

* Provides simple static functions that make Java a *whole* lot easier to use:

```java
println("Hello");
```
rather than 
```java
System.out.println("Hell-o");
```
Other static functions:
```java
String quakeText = readFile("4.5_week.atom");

List<String> words = readFileAsLines("dict.txt");

writeFile("file.txt", str);

writeFileAsLines("lines.txt", list);

printf("%d words in %s\n", words.size(), path);

print("Hello");

String s = readLine();  // Read a line of text from the console

parseInt/Long/Float/Double/Boolean()
```

* [PMD](https://pmd.github.io/) support, including a tailored set of rules (`cs106.ruleset`).
