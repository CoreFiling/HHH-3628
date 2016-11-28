# Patch for HHH-3628

This is a modified class from Hibernate with a fix for HHH-3628. The
hi-lo optimizer cannot otherwise be used from multiple processes against
the same database.

To build:

- Import this project into Eclipse and wait for Ivy resolution.
- File -> Export -> JAR file.
- Select this project's only package and no resources.
- Use any ZIP tool to copy the class files from the exported JAR into
  hibernate-core-4.3.10.Final.jar, overwriting the original classes.
