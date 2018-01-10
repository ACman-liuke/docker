1、sudo docker images: 可以看到一个叫 tenbay:latest  ID为81e16b1f036a，大小为2.095GB的镜像，这是作为编译环境的基础镜像，已经可以编译出x86的包；
2、每一个容器项目都在data目录下建一个目录，如/data/x86
3、每一个容器项目目录里面的结构x86所示：docker-compose.yml，script/ , work/
   docker-compose.yml是构建，启动停止容器必要的配置文件，docker-compose命令必须要的文件；
   script目录是存放容器启动时要执行的脚本的目录；
   work目录是宿主机映射到容器里的目录, 建议用户将需要保存的数据都放到这里；
4、新建容器项目，可以直接复制x86文件件为新项目的名称即可；项目文件夹名称必须与docker-compose.yml文件里的名字一致，不然docker-compose不能控制.
