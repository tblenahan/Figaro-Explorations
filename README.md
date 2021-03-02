# Figaro-Explorations
Becoming familiar with Scala's probabilistic programming language/library Figaro

## Installation for execution in notebook environment

**Note:** first I will list the software environment I am running this repo's notebook(s) in then I will list/link the instructions for how to install each of these

### From Jupyter Notebook: Help -> About (03/02/21)
  - Almond 0.10.0
  - Ammonite 2.1.4
  - Scala library version 2.12.11 -- Copyright 2002-2020, LAMP/EPFL and Lightbend, Inc.
  - Java 15.0.1
  
### Required installations
  - [Java](https://adoptopenjdk.net/releases.html?variant=openjdk15&jvmVariant=hotspot) (JVM)
  - [Almond](https://almond.sh/docs/quick-start-install) (Scala kernel for Jupyter)
 
### For actually executing Figaro programs
 ```
import coursierapi._
interp.repositories() ++= Seq(
  MavenRepository.of("https://mvnrepository.com/artifact/com.cra.figaro/figaro"),
 )
import $ivy.`com.cra.figaro:figaro_2.12:5.0.0.0`
```

**!Important! Note:** Figaro is sensitive to the Scala [version](https://mvnrepository.com/artifact/com.cra.figaro/figaro) being used
