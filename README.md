# Synthea-project
## Getting Started
## Prerequisites
**System Requirements**:
- SyntheaTM requires Java JDK 11 or newer. I used Java JDK 17. You can find it on the [Oracle website](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html).
- [Git](https://git-scm.com/downloads) is a plus to run your commands
- [Visual Studio Code](https://code.visualstudio.com/) to make changes were necessary
## Installation
To clone the SyntheaTM repo, then build and run the test suite (on Git Bash):
```
git clone https://github.com/synthetichealth/synthea.git
cd synthea
./gradlew build check test
```
## Changing the default properties
I used CSV as my data format of choice. This required adjusting the file in VS Code.
First, I searched for Synthea in File Explorer and then followed the path `src/main/resources/synthea.properties` to edit the properties file.
**Search for this line:**\
```
exporter.csv.export = false
```
**Change it to:**
```
exporter.csv.export = true
```
This ensures Synthea will generate data in `/output/csv/` each time you run it.
