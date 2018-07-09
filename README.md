## Designing Smart City Mobile Applications: An Initial Grounded Theory

### Case Study

[Link](url) and ![Image](src)

#### Interview Questions
###### Card 1: Requirements
1. Could you talk about the software development team members of the project?
2. How long did this project last?
3. Where did the idea of the app come from? Did you think about the smart city context initially?
4. How were the requirements defined?
5. Was there any documentation?
6. Did you analyze the main challenges of the project from a development perspective? If so, how did you mitigate them?
7. Could you cite any problem encountered and how did you resolve it?
8. [*Show a list of non-funcional requirements and ask the following questions for each one:*] 
For example: Performance:
a. Why performance was [not] crucial? 
b. How did you deal with performance issues?
c. How was it specified? How was it modeled in the architecture? How was it implemented? What aspects of testing were applied to ensure performance?

###### Card 2: Software Architecture


###### Card 1: Mobile Development


**********

### Reversed-Engineering Architecture

> **Steps**

    - Get the apk file
    - Use COVERT tool to generate the intermediate code (*file.xml*)
    - Add *file.xml* into *ACME-Generator* folder with *file.apk*
    - Execute the comand line to generate *file.acme*
    - Open *file.acme* in ACME STUDIO
    
##### APk & COVERT

```sh
$ java -jar apktool.jar d K-9\ Mail_5.207_apk-dl.com.apk -f
```

| Apk converter | Site |
| ------ | ------ |
|Apkbucket |  [apk-downloader](https://apkbucket.net/apk-downloader) |
|Apktool |  [apk-dl](http://apk-dl.com) |
|Project | [Project](http://www.ics.uci.edu/~seal/projects/covert/index.html) |
|Tutorial | [Tutorial](http://www.ics.uci.edu/~seal/projects/covert/COVERT%20User%20Manual_v2.0.pdf) |
|ACME-Generator | [ACME-Generator](https://github.com/arsadeghi/ACME-Generator) |

- Add o file *example.apk* em Covert folder
- Comando: ```sh $ ./covert.sh folder ```
- Output: *example.xml* (locaded in folder/analysis/model/example.xml)

##### ACME-Generator
- Add a saída do covert na pasta ACME-Generator-master
- Comando: ```sh run.py ./apps/example.apk ./resources    ```
- Output: *example.acme*

##### ACME STUDIO
- Create a new project
- Add file *example.acme* in ACME workspace
- Refresh project

**********
