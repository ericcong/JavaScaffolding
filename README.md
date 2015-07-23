# JavaScaffolding

Lightweight bootstrap and utility scripts for tiny Java projects

## Setup

1. Clone this repository
2. Add the cloned repository into your PATH by inserting `PATH=$PATH:${the repository's path}` into `~/.bash_profile`
3. Install `ivy` by `brew install ivy`

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

### Init a class

Under `src`, run:

`init-class $package_name.$class_name`

For example: `init-class foo.bar.Test` will create the directory `foo/bar` under the current directory and the file `Test.java` with package information.

### Get dependency

Go to `lib` directory, use this command:

`get-jar groupId articleId version`

Then it will download the library along with all its dependencies into the current directory.

### Build Jar

`make`

This will generate a jar file that includes all compiled class files for the source codes in `src` and jar files in `lib`

The entry class is `src/$name`

### Package

Feel free to add packages into `src`
