# Dokumentasi DSpace TA 25 
------
| Source | Download |
| ------ | ------ |
| Source Code | [https://drive.google.com/drive/folders/1OQanqnTgLj3rOMibL9G-ep9MYqTr6hdk][PlDb] |
| User Manual | [https://drive.google.com/drive/folders/1OQanqnTgLj3rOMibL9G-ep9MYqTr6hdk][PlGh] |

## Pre-requisite Software
------
| Software | Download |
| ------ | ------ |
| Java SE Development Kit 8u202 | [https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html#license-lightbox][PlDb] |
| Apache Maven 3.6.3 | [https://repo.maven.apache.org/maven2/org/apache/maven/apache-maven/3.6.3/apache-maven-3.6.3-bin.zip][PlGh] |
| Apache Ant 1.10.12 | [https://archive.apache.org/dist/ant/binaries/apache-ant-1.10.12-bin.zip][PlGd] |
| Apache Tomcat 9 x64 | [https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.0.M13/bin/apache-tomcat-9.0.0.M13-windows-x64.zip][PlOd] |
|  PostgreSQL 9.4.26 windows x86-64 | [https://www.enterprisedb.com/postgresql-tutorial-resources-training?uuid=91f8264f-8a2d-434a-9559-4dfa9b3b80b1&campaignId=701380000017oAXAAY][PlMe] |
| Git for Windows | [plugins/googleanalytics/README.md][PlGa] |

## Pre-requisite Mirage 2
-----

### Bower 
Install [Bower](http://bower.io/) menggunakan command berikut
```bash
    npm install -g bower
```
Cek versi Bower dengan perintah berikut
```bash
    bower -version
```

### Grunt
Install [Grunt](http://gruntjs.com/) menggunakan command berikut
```bash
    npm install -g grunt && npm install -g grunt-cli 
```
Cek versi Grunt dengan perintah berikut
```bash
    grunt -version
```

### Compass ###
Install Sass menggunakan command berikut
```bash
    gem install sass -v 3.3.14
```
Install Compass menggunakan command berikut
```bash
    gem install compass -v 1.0.1
```
Cek versi Sass dan Compass dengan perintah berikut
```bash
    sass -version
```
```bash
    compass --version
```

## Instalasi
------
Download Source Code dan ikuti langkah yang disediakan pada User Manual yang terlampir. Buka direktori penyimpanan source code (Disarankan untuk menyimpan folder pada direktori C:/DSpace)
```bash
    cd C:/DSpace
```
Compile dengan menggunakan perintah berikut
```bash
    mvn package -Dmirage2.on=true -Dmirage2.deps.included=false
```
Pindah ke direktori instalasi
```bash
    cd dspace/target/dspace-installer
```
Lanjutkan dengan menjalankan perintah berikut
```bash
    ant fresh_install
```
Buka DSpace di lokal anda menggunakan alamat berikut 
```bash
    localhost:8080/xmlui
```


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
