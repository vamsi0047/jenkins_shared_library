1. vars -- this folder container all the groovy scripts which can be called inside the actual pipeline
2. resources -- this folder can contain files will can be used inside pipeline like json files, yaml files ...etc
3. src -- this folder will container the source code which can used by files in vars directory. (local code or custom classes)

vars:
  the groovy files inside the vars folder can be access inside pipeline by call the groovyfile
  ex: -
     sonar.groovy file contains below methods
     call()
     sonarreport()
        
      in pipeline I will call with sonar() or sonar.call() and second method with sonar.sonarrepot().
      if the method name is call you don't need to mention method name explicitly.

 
