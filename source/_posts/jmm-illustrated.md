"title": "A Note on Java Memory Model",
"date": "2017-12-17 11:18:42",
"tags": ["java", "jmm","java memory model", "computer architecture", "memory","thread","os","PL/Compilers"],
"categories": ["Java"],
"toc" : true
;;;



### Preface 
Java Memory Model(abbr. JMM later) has been and will alway be one of the most fundamental and hardest area to understand. Yet, in learning java language, we just can not circumvent this topic. Without deep understanding of Java Memory Model, it is hard to write correct concurrent programs in java. <!-- more -->However, mastering JMM needs significant system level knowledge like computer architecture, operating system, compilers, etc. This note mainly aims to record the process how I understand and learn this topic over time. 

### Disclaimer
This topic will be update to date and it is not ganranteed that opinions given here are correct. Origins of the references used in this paper will be given [References](#references). 


### What is the exact definition, and to what extent should we master it
What does JMM do exactly, and why does java have its language level memory model? Before delving into any specifics of Java Memory model, we need to be able to answer thoes two questions. After extensive reading and thinking, I can only answer thoes two questions by citations from gurus in this field. Put it simply and bluntly, I think the answer to the first question in my opinion could be:

* In storage-savvy languages, the memory models appear to answer a simple question:"What values can a particular read observe?"<sup>[1](#ref-1)</sup>

and the answer to the second may be:

* Java have built-in support for synchronizaiton and is claimed to be cross-platform, which means it should abstract aways the low level details and promote synchronization into language level.

### Prerequisites
#### Reorders
If all the instructions were to be executed sequentially, it will be a lot easier for us to understand the outcome of a program. However, it is just not the case. Compilers and Operating Systems are free to reorder instructions so that our code is executed more efficiently. Understanding all kinds of reorders may help us comprehend the design behind the JMM. 

##### Compiler Optimization
##### Out-of-order Execution








### Some key points in understanding the JMM Model###
* Understanding the **built-in** synchronization mechanism
* Understanding the **volatile** keyword, its influence on memory visibility as well as its impact on instruction reordering
* Unserstanding the semantics of **final** keyword and its influence on object initialization








<a name="references"></a>
### References
1. <a name="ref-1" href="https://shipilev.net/blog/2014/jmm-pragmatics/">Java Memory Model Pragmatics</a>
2. <a name="ref-2" href="http://www.cs.umd.edu/~pugh/java/memoryModel/jsr-133-faq.html">Famous JSR133 FAQ</a>
