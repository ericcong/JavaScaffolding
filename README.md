# JavaScaffolding

Lightweight bootstrap and utility scripts for tiny Java projects

## Scaffolding structure

```
./
|- Makefile             # The make recipe
|- lib/                 # Dependency jar files
|- src/                 # Source directory
   |- $name.java        # Entry class
   |- assets/           # Static files
```

## Usage

### Init a Java project

`init-java $name`

For example: `init-java Foo` will create a new project under current directory.

### Get dependency

Go to `lib` directory, use this command:

`get-jar groupId articleId version`

Then it will download the library along with all its dependencies into the current directory.

### Build Jar

`make`

This will generate a jar file that includes all compiled class files under `src` and jar files under `lib`

The entry class is `src/$name`

### Package

Feel free to add packages into `src`

