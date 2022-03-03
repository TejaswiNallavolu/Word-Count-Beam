# java-word-count-beam

## Get the example code
`PS> mvn archetype:generate
 -D archetypeGroupId=org.apache.beam
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples 
 -D archetypeVersion=2.36.0 
 -D groupId=org.example 
 -D artifactId=word-count-beam 
 -D version="0.1" 
 -D package=org.apache.beam.examples 
 -D interactiveMode=false`
 
 ### This will create a word-count-beam directory that contains a pom.xml and several example pipelines that count words in text files.
-  `PS> cd .\word-count-beam`
-  `PS> dir`
- `PS> dir .\src\main\java\org\apache\beam\examples`

## Get sample text
- In the word-count-beam directory, create a file called sample.txt.
- Add some text to the file. For this example, you can use the text of Shakespeare’s [Sonnets](https://github.com/TejaswiNallavolu/java-word-count-beam/blob/master/word-count-beam/input.txt).

## Run WordCount Using Maven
`PS> mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount`
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner`
 
 ## Inspect the results
 `$ ls counts*`
 
