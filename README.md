# WORKSPACE-CS106

This is the Eclipse workspace that is to be used for CS106, CS165, and CS180.  It includes:
*  Eclipse preferences set to support easier coding in Java.
*  The **JavaCoreTemplate** project:  make a copy of this project when starting each assignment.  The JavaCoreTemplate project supports the following goodies:

&nbsp;

# Main

Includes `Main.java`, with a `main()` function that is ready to go, and has useful classes statically imported.

# println
Eliminate the EVIL `System.out.` and just use:
```java
println("Hello");
```
# readLine
Read a line of text from the console:
```java
String s = readLine();
```

# readFile
Read a whole file into a String with one line of code:
```java
String quakeText = readFile("4.5_week.atom");
```
# readFileAsLines
Read a file into a list of Strings:
```java
List<String> words = readFileAsLines("dict.txt");
```
# writeFile
Write a string to a file:
```java
writeFile("file.txt", str);
```
# writeFileAsLines
Write a list of strings to a file:
```java
writeFileAsLines("lines.txt", list);
```
# printf
printf w/o requiring `System.out.` in front:
```java
printf("%d words in %s\n", words.size(), path);
print("Hello");
```
# parseInt/Long/Float/Double/Boolean
Parse ints, floats, etc w/o having to put `Integer.` in front:
```java
int age = parseInt(text);
```

# asList
```java
var list = asList("This", "That", "And the other");
```

# range
Use range() to loop in a pythonic manner:
```java
for (var x : range(10))
	println("Hello " + x);
```

# join, substringsBetween, substringBefore, substringAfter, reverse, and more
JavaCoreTemplate includes the wonderful [`StringUtils`](https://commons.apache.org/proper/commons-lang/apidocs/org/apache/commons/lang3/StringUtils.html), which has `join`, `substringsBetween`, `reverse`, etc.  For example:
```java
String[] titles = substringsBetween(quakesXml, "<title>", "</title>");
```

# PMD
[PMD](https://pmd.github.io/) support, including a tailored set of rules (`cs106.ruleset`).

&nbsp;
# STATIC IMPORT OF CORE FUNCTIONALITY
JavaCoreTemplate's `Main` class already has the `Core` functionality statically imported.  To add `Core` functionality to other classes, add the following static import at the top of the `.java` file:
```java
import static sbcc.Core.*;
```
&nbsp;
# TO USE
1.  If you are using the SBCC Student Desktop VDI:
    1.  Download [workspace-cs106-v5.zip](https://github.com/ProfessorStrenn/workspace-cs106/releases/download/v5.0/workspace-cs106-v5.zip)
    2.  In Windows Explorer, copy the .zip file to the N:\ drive (CSnebula).
    3.  Right-click the .zip file, select **7-zip | Extract Here**.  If asked about overwriting files, click Yes to All.
    4.  Double-click the N:\CompSci\launchers\Eclipse CS106 shortcut.  This will launch Eclipse and point it at N:\workspace-cs106_v5.
    5.  If you get an "older version warning", check the "Do not warn again..." box and click Continue.

2.  If you are on your own computer:
    1.  Download [workspace-cs106-v5.zip](https://github.com/ProfessorStrenn/workspace-cs106/releases/download/v5.0/workspace-cs106-v5.zip)
    2.  Unzip the workspace where you like.
    2.  File | Switch Workspace | Other...
    3.  Navigate to where you unzipped workspace-cs106-v5.  ** NOTE: By default, Windows extracts and extra level of folder.  I.e. your_folder/workspace-cs106-v5/workspace-cs106-v5.  Double check this.  If you have the "extra level", be sure to navigate to the inner level:  your_folder/workspace-cs106-v5/workspace-cs106-v5.
    4.  Click OK, then click OK again.

4.  If you haven't already done so, check out the [time-saving features that the workspace offers](#WORKSPACE-CS106)
