# Java-Assignment-003

### Input, Packages, Imports, and a static Method

## PART 1 - Build an External Package (JAR short for Java Archive)

A Jar is really just a Zip file with some added Metadata (i.e. data about data). They are organized much the same way file systems are organized, think folders nested in folders with importable Java classes being the files in those folders. So if you have a folder hierarchy like **edu/redwoods/cis12** and you had several Java files in the cis12 subfolder named **Class1** and **Class2** you could Zip it up into a **.jar** file, import it into your IntelliJ project, and then import those classes like so:

```
import edu.redwoods.cis12.Class1;
import edu.redwoods.cis12.Class1;
```

This is a slight over-simplification because you would also have to include a **package** directive at the top of your Java classes, and you should add additional package metadata, but the comparison is pretty close to reality.


1. Watch the below linked video, and follow along on how we build a **Java Archive** artifact (**jar**) from a GitHub project.
    * [Jar file build from GitHub Project](https://redwoods.us-west-2.instructuremedia.com/embed/517c63e3-9624-4880-a46f-7eea3efe338a)
1. If you didn't already, attempt to build the artifact/jar file while watching the video, try to build **the jar file** yourself now!
    * [Metadata Extractor Code on GitHub](https://github.com/drewnoakes/metadata-extractor)
1. Watch the below linked video, and follow along to import an external **jar** file into your project!
    * [Import External Jar into your Project](https://redwoods.us-west-2.instructuremedia.com/embed/92f5cfd8-59f3-48b8-bbfe-a16c664625ac)
1. If your artifact build/creation step was successful, see if you can import your build of the metadata jar file into Java-Assignment-003 after you start PART 2 below!

## PART 2 - Implementation

Just like you do every week now!!!

* **Fork** my assignment repo
* Use IntelliJ to **clone** your fork locally
* Use IntelliJ to create a local **feature branch**
* Complete the following assignment:

Your assignment is to use Built-In java classes to:

1. Import the following java Built-In classes from the **java.nio** and **java.util** packages respectively.
    * ```
      java.nio.file.Paths;
      java.util.Scanner;
      java.nio.file.Path;
      ```
1. Read a **jpg file path** from the user.
     * HINT 1: Create a **Scanner** object instance and use it to read a string.
     * HINT 2: Use **Paths** class to get a path from your input!
         * Google java.nio.file.Paths for help OR [Look for examples HERE](https://www.geeksforgeeks.org/java-nio-file-paths-class-in-java/)
1. From your path object call a **method** that converts the file path to a **File** type object (**Cause that's what the provided getHiddenSecret method declares as its parameters**).
1. Pass the file object as an argument to the given **getHiddenSecrets** method.
1. Run the program and type in the path for our sample image, and record the GPS coordinates in the output.
  ![Ollie the Otter Image](images/OllieTheOtter.jpg)
   ![GPS Coordinates](C:\Users\17076\IdeaProjects\Java-Assignment-003\images\GPScoordinates.jpeg)

    * HINT: the path can be relative to the project directory, maybe use the string in the example above :-)
1. Look up the latitude and longitude coordinates in any online map you can find via Google.
1. Screenshot the map and add it into the **images** folder of this project.
1. Last add image markdown below this line to load your map image (Hint: Example image Markdown is just a couple lines above this).

## PART 3 - Code Scanning and Interpretation

* Look at the getHiddenSecrets method and identify the following parts by editing this README.md and providing your answers:
    * What is the **access modifer** (e.g. public, private, protected)? Public
    * Is it a **Class method** or an **object Instance method**, how do you know? The method "getHiddenSecrets" is a class method. The getHiddenSecrets method is a class method, as it is declared using the static keyword. This means that it can be called without creating an instance of the class and it operates directly on the class itself. Class methods are also commonly referred to as "static methods".
    * What is its **return data-type**? it doesnt have one its void
    *  The method getHiddenSecrets requires 1 argument to be called, which is a File object. This means that when the method is called, it needs to be passed a File object as a parameter. The method takes 1 parameter, which is of type File.* Scan line by line through the code and try to determine how it works?
    * What is familiar to you? nothing lol
    * What is not familiar to you? all of it
    * Do the **for** loops make sense, and if so, tell me what you think they do? The two "for" loops in the code are used to iterate over the metadata obtained from the image file. The first "for" loop iterates over the "directories" in the metadata, and the second "for" loop iterates over the "tags" in each directory. The code then prints the name of the directory, the tag name, and the tag description.

## PART 4 - Turn in

### Same as the last 2 Weeks!

* When completed, use your IDE to **Commit** and **Push** your **feature branch** back to your GitHub Account's **fork** of Java-Assignment-003.
* From your GitHub account's feature branch, issue a New **Pull request** from your **feature branch** to the instructor's fork
* Save the *Pull Request URL* to submit to your Canvas assignment.
