# WORKSPACE-CS106-V3

Eclipse workspace used for CS106, CS165, and CS180.  It includes:
*  The **JavaCoreTemplate** (see below) project:  make a copy of this project when starting each assignment.
*  Eclipse preferences set to support easier coding in Java.


# JavaCoreTemplate

Includes:
* `Program.java`, with a `main()` that is ready to go, and has useful classes statically imported.

* Provides simple static functions that make Java a *whole* lot easier to use:

```java
println("Hello");
```
rather than 
```java
System.out.println("Hello");
```
Other static functions:
```java
String quakeText = readFile("4.5_week.atom");  // Read a whole file into a String with one line of code.

List<String> words = readFileAsLines("dict.txt");  // Read a file into a list of Strings.

writeFile("file.txt", str);  // Write a String to a file.

writeFileAsLines("lines.txt", list);  // Write a list of strings to a file.

printf("%d words in %s\n", words.size(), path);

print("Hello");

String s = readLine();  // Read a line of text from the console

parseInt/Long/Float/Double/Boolean()  // Parse ints, floats, etc w/o having to put Integer. in front.
```

* `commons-lang3`:  With the wonderful `StringUtils`, which has `join`, `substringsBetween`, `reverse`, etc.  For example:
```java
String[] titles = substringsBetween(quakesXml, "<title>M ", "</title>");
```

* [PMD](https://pmd.github.io/) support, including a tailored set of rules (`cs106.ruleset`).

# TO USE
1.  Download [workspace-cs106-v3.zip](https://github.com/ProfessorStrenn/workspace-cs106-v3/releases/download/initial_commit/workspace-cs106-v3.zip) and unzip it.
2.  Launch Eclipse.
3.  File | Switch Workspace | Other...
4.  Navigate to where you unzipped workspace-cs106-v3.
5.  Click OK, then click OK again.
