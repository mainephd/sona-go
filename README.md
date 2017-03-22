# Sonago
Provides a convenient way to convert a coverage file that is generated by `go test -cover` to
the generic coverage xml format that can be digested by Sonar which is documented [here](https://docs.sonarqube.org/display/SONAR/Generic+Test+Data).

# Usage
Sonago will look for a file look in the current directory for a file with the name of `gover.coverprofile` and will produce a file with the name of `coverage.xml` when it completes.

This behavior can be modified by passing in command line flags to specify the file names.

```bash
sonago -inputfile=myconverageprofile.out -outputfile=mycoverageresults.xml
```
