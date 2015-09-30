# GoMoDaMo 

## Go MongoDB Data Modeling Tools

Gomodamo is a command line tool written in Go that will generate common data modeling functions by analyzing a set of types defined by the developer.  

Another way of thinking of it is, Gomodamo takes your types and makes them into the "m" in "mvc". 

### General Design Approach

gomodamo will be installed, which should result in a command line utility named gmdm being available.  The developer will create a package structure with a top level package for the over all data model, and sub packages for each data type contained in the model.  

```
/datamodel
    - datamodel.go // contains data model configuration
    /