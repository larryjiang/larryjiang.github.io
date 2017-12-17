"title": "A Note on Java Memory Model",
"date": "2017-12-17 11:18:42",
"tags": ["java", "jmm","java memory model", "computer architecture", "memory","thread","os","PL/Compilers"],
"categories": ["Java"],
"toc" : true
;;;



### Preface 
Java Memory Model(abbr. JMM later) has been and will alway be one of the most fundamental and hardest area to understand. Yet, in learning java language, we just can not circumvent this topic. Without deep understanding of Java Memory Model, it is hard to write correct concurrent program in java. <!-- more -->However, mastering JMM needs significant system level knowledge like computer architecture, operating system knowledge, compilers, etc. This note mainly aims to record the process how I understand and learn this topic over time. 

### Disclaimer
This topic will be update to date and it is not ganranteed that opinions given here is correct. Origins of the references used in this paper will be given [References](#references). 


### What is the exact definition, and to what extent should we master it

<a name="references"></a>
### References
