# Sarras

**Note:** IN PROGRESS ... NOT IMPLEMENTED YET, STAY TUNED!!!

## What is Sarras?

**Sarras** is [Reflection Configuration File](https://github.com/oracle/graal/blob/master/substratevm/REFLECTION.md) Generator tool for **Graal Substrate VM** by Static and Dynamic Profiling of Java Applicatons.

See the technical discussion about the approach: https://github.com/oracle/graal/issues/476

### Static Profiling

Parses bytecode of all classes in the given jar, introspectes reflective calls (class/method/field accesses through reflection, etc ...) and adds their configurations to the generated reflection configuration file.

### Dynamic Profiling

Attaches to a regular Java application (not from native image) as Java agent and intercepts reflection calls (also includes `Class.forName(...)` and `ClassLoader.loadClass(...)` calls). So it can collect information at runtime about which classes/methods/fields are accessed/referenced through reflection and adds their configurations to the generated reflection configuration file.

## Where the Name `Sarras` Come From?
> Sarras is a mystical island to which the Holy Grail is brought in the Arthurian legend. 

See [Wikipedia](https://en.wikipedia.org/wiki/Sarras) for more details.
