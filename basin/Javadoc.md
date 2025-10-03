A tool that parses source code utilizing specially formatted comments in order to generate [[API Documentation|API documentation]] for classes and class members. The specially formatted comments are named [[Doc Comments|Doc comments]].

Common block tags in Javadoc include:

- `@author`: specifies an author.  `class`
- `@version`: version number. `class`
- `@param`: denotes a parameter's description. `method, constructor`
- `@return`: describes the value or object return by the method. `method`
- `@see`: refers any readers to relevant websites or class members. `all`

By default, Javadoc will not include private class members in the API. Use the `-private` flag at Javadoc's execution to include them.

---
#computer-science #java 