[Back](https://saner-decay-factors.github.io/)

# Software Metrics List

| Attribute   | Software Metric                       | Description                                                                                                                                               | Improves When |
|-------------|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Cohesion    | Lack of Cohesion in Methods 2 (LCOM2) | Number of method pairs that do not share attributes, minus the number of method pairs that share attributes.                                              | Decreases     |
|             | Lack of Cohesion in Methods 3 (LCOM3) | Treats each method pair as an individual entity, and determines the difference between the amount of similar and different pairs.                         | Decreases     |
|             | Tight Class Cohesion (TCC)            | The number of directly connected visible methods in a class divided by the number of maximal possible connections between the visible methods of a class. | Increases     |
| Coupling    | Coupling Between Object (CBO)         | The number of classes coupled to the analyzed class.                                                                                                      | Decreases     |
|             | FANIN                                 | The number of external classes that invoke methods from the analyzed class.                                                                               | Decreases     |
|             | FANOUT                                | The number of external method invocations made by the analyzed class.                                                                                     | Decreases     |
| Inheritance | Base Classes (IFANIN)                 | The number of immediate base classes and interfaces.                                                                                                      | Decreases     |
|             | Number of Children (NOC)              | The number of immediate subclasses to the analyzed class.                                                                                                 | Decreases     |
|             | Depth of Inheritance Tree (DIT)       | The number of nodes between the root of the inheritance tree and the analyzed class.                                                                      | Decreases     |
| Complexity  | Cyclomatic Complexity (CC)            | Measure of the complexity of a module’s decision structure.                                                                                               | Decreases     |
|             | Essential Complexity (ev(G))          | Measure of the degree to which a module contains unstructured constructs.                                                                                 | Decreases     |
|             | Maximum Nesting (MAxNEST)             | Maximum nesting level of control constructs.                                                                                                              | Decreases     |
|             | Weighted Methods per Class (WMC)      | The sum of the cyclomatic complexity of the methods of a class.                                                                                           | Decreases     |
|             | Number of Methods (NM)                | The number of non-inherited methods declared in the analyzed class.                                                                                       | Decreases     |
| Size        | Physical Lines (NL)                   | The number of physical lines in the class.                                                                                                                | Decreases     |
|             | Blank Lines of Code (BLOC)            | The number of blank lines of code in the class.                                                                                                           | Decreases     |
|             | Source Lines of Code (LOC)            | The number of lines containing source code in the class.                                                                                                  | Decreases     |
|             | Declarative Lines of Code             | The number of lines containing declarative source code in the class.                                                                                      | Decreases     |
|             | Executable Lines of Code              | The number of lines containing executable source code in the class.                                                                                       | Decreases     |
|             | Lines with Comments (CLOC)            | The number of lines containing comments in a class.                                                                                                       | Increases     |
|             | Semicolons                            | The number of semicolons in a class.                                                                                                                      | Decreases     |
|             | Statements                            | The number of statements in a class.                                                                                                                      | Decreases     |
|             | Declarative Statements                | The number of declarative statements in a class.                                                                                                          | Decreases     |
|             | Executable Statements                 | The number of executable statements in a class.                                                                                                           | Decreases     |
|             | Comment to Code Ratio                 | The ratio of comment lines to code lines in a class.                                                                                                      | Increases     |
|             | Instance Variables (NIV)              | The number of instance variables in a class.                                                                                                              | Decreases     |
|             | Instance Methods (NIM)                | The number of instance methods in a class.                                                                                                                | Decreases     |
|             | Methods                               | The total number of methods, including inherited ones, in a class.                                                                                        | Decreases     |
|             | Local Default Visibility Methods      | The number of local methods with default visibility in a class.                                                                                           | Decreases     |
|             | Average Number of Lines               | The average number of physical lines between methods of a class.                                                                                          | Decreases     |
|             | Average Number of Blank Lines         | The average number of blank lines of code between methods of a class.                                                                                     | Decreases     |
|             | Average Number of Lines of Code       | The average number of lines of source code between methods of a class.                                                                                    | Decreases     |
|             | Average Number of Lines with Comments | The average number of lines containing comments between methods of a class.                                                                               | Increases     |
|             | Class Methods                         | The number of class methods in a class.                                                                                                                   | Decreases     |
|             | Class Variables                       | The number of class variables in a class.                                                                                                                 | Decreases     |
|             | Private Methods (NPM)                 | The number of local private methods in a class.                                                                                                           | Decreases     |
|             | Protected Methods                     | The number of local protected methods in a class.                                                                                                         | Decreases     |
|             | Public Methods (NPRM)                 | The number of local public methods in a class.                                                                                                            | Decreases     | 