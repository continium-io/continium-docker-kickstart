# Docker Kickstart

## Docker Nedir, Ne İçin Kullanılır?

Docker, uygulamaların farklı ortamlarda çalıştırılması sürecinde kullanılan bir platformdur. Uygulamamızı derler, ölçeklendirir, paketler ve dağıtmamızı sağlar. 

Docker içerisinde barındırdığı konteynerleştirme yapısını ve Docker Hub üzerinden indirilen image’ ları kullanarak ürünü farklı işletim sistemi, versiyon ve environment’ larla birbirinden izole şekilde çalıştırır.
Docker yeterli kaynak ve gerekli yapılandırmalar ile birlikte kullanıldığında, yapısal problemleri ortadan kaldırarak uygulamalarımızı stabil bir şekilde çalışabilecek hale getirir.

## Containerization (Konteynerleştirme) Nedir?

Konteynerleştirme, bir sunucu üzerindeki işletim sisteminin diğer konteynerler tarafından paylaşılması demektir. Birbirinden farklı uygulamalar, dağıtımlar ve envrionment’ ları birbirinden izole şekilde çalıştırır. 


## Gereksinimler

```
Docker
Ubuntu Bionic 18.04 (LTS)
Diğer İşletim Sistemleri için https://docs.docker.com/engine/install/ adresinden bilgi alabilirsiniz. 
```

## Docker Kurulum

*Ubuntu Bionic 18.04:*
```
$ sudo apt-get remove docker docker-engine docker.io containerd runc
$ Curl -fsSL https://get.docker.com -o get-docker.sh
$ sudo sh get-docker.sh

```

### Docker Color Örnek

```
 cd "color_html_example"
 Docker build -t myimage .
 Docker run -d -p 8888:88 -e AUTHOR = "red" myimage 
 https://localhost:8888' e giderek görüntüleyebiliriz.
```
### Docker Compose Örnek
```
 cd "docker_compose"
 Docker-compose up -d
 https://localhost:5000 ' e giderek görüntüleyebiliriz.
```

### Java Örnek
```
 cd "java_example"
 Docker build -t hello .
 Docker run hello
```

