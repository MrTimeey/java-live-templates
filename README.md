# Custom Live Templates for Java

These are my custom [IntelliJ IDEA Live Templates](https://www.jetbrains.com/help/idea/using-live-templates.html) for Java that i'm currently using.

I though some of them might be helpful for others so i shared them. If you got other cool custom Java live templates which you want to share, feel free to contribute!

## Export and Import
All these custom live templates are placed in a custom group. According to [sharing live templates](https://www.jetbrains.com/help/idea/sharing-live-templates.html) I've selected only the live templates and created an export. You can import these settings if you want to get all these templates. 
Furthermore I've added the templates config file from the IDEA settings. Copy this file to your IDEA settings directory and you are ready to go.

If you just want to add a single live template you can also create it manually.

## Java
The live templates are all applicable in Java classes.

### JUnit Test Method
Simple test method generation with imported `assertThat` from AssertJ.

![Generate simple test method](test_method/example.gif)

Abbreviation: __test__
Template text:
```java
@org.junit.jupiter.api.Test
public void test$Function$() {
    org.assertj.core.api.Assertions.assertThat("").isEqualTo("false");
}
```
Options:
- [x] Reformat according to style
- [x] Use static import if possible
- [x] Shorten FQ names

### Create SLF4J-Logger
Creates SLF4J logger and adds the static imports.

![Generate simple test method](slf4j_logger/example.gif)

Abbreviation: __log__

Template text:
```java
private static final org.slf4j.Logger LOGGER = org.slf4j.LoggerFactory.getLogger($CLASS$.class);
```
Options:
- [x] Reformat according to style
- [ ] Use static import if possible
- [x] Shorten FQ names

## Contributing
Want to add some more live templates? Send a pull request or open a ticket!