GradleDocPrintScript
====================

Shell script to convert code listing colors in Gradle PDF to be printer friendly.
Script uses "pdftk" and "mimetype" command. Be shure you have them installed on your system.
Written and tested with version 2.0 of the Gradle user guide.

Steps to do:

1. Download the gradleDocColors.sh script
2. Go to http://www.gradle.org/documentation and download the userguide.pdf
3. Set script to be executable
```chmod +x gradleDocColors.sh```
4. Start the script with the userguide.pdf as parameter
```./gradleDocColors.sh userguide.pdf```
5. The script will then uncompress the pdf, change it's colors and then compresses it again
6. New document is named as the original but with prefix "print-"

Original code style:

![original style screenshot](https://raw.githubusercontent.com/d4nj1/GradleDocPrintScript/master/originalStyle.png)

Java code style: (default)

![java style screenshot](https://raw.githubusercontent.com/d4nj1/GradleDocPrintScript/master/javaCodeStyle.png)

Groovy code style: (changeable in script)

![groovy style screenshot](https://raw.githubusercontent.com/d4nj1/GradleDocPrintScript/master/groovyCodeStyle.png)
