# Docker

可以將運行環境包裝到容器(Container)

1.  Source Code, PHP8, Nginx, MySQL8, Redis 6.2
2.  Source Code, PHP7.4, Apache, MySQL 5.6
3.  Source Code, PHP7.2, Apache, MySQL 5.6

## 高耦合容器

由於將服務都包裝到單個容器當中的彈性較差，
因此另一種做法是可以將內容拆分到個別單獨的容器當中。(解耦)

1. Volume(Source Code) -> PHP, Webserver (Apache / Nginx)
2. Volume(mysql-data) -> MySQL

## Docker 組成

Dockerfile -> Doceker Image -> Container

Dockerfile 是一個文件檔，有關如何構建 Docker Image 的說明
Docker Image 是一個唯讀的執行檔，包括運行程式所需的內容，如程式碼的依賴項、環境變數。
Container 真正運作的執行檔。(runtime instance of an image)

Image, Container 類似 Class, Object 的關西
