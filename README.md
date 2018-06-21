# Designing Smart City Mobile Applications: A initial Grounded Theory

### CASE STUDY

[Link](url) and ![Image](src)

**********

### EXPERIMENTAL STUDY

> **Steps**

    - Get the apk file
    - Use COVERT tool to generate the intermediate code (*file.xml*)
    - Add *file.xml* into *ACME-Generator* folder with *file.apk*
    - Execute the comand line to generate *file.acme*
    - Open *file.acme* in ACME STUDIO
    
### APk & COVERT

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

### ACME-Generator
- Add a saída do covert na pasta ACME-Generator-master
- Comando: ```sh run.py ./apps/example.apk ./resources    ```
- Output: *example.acme*

### ACME STUDIO
- Create a new project
- Add file *example.acme* in ACME workspace
- Refresh project

**********
