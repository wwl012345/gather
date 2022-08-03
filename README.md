# gather
**Linux服务器信息收集脚本**

### 一、功能介绍
#### 1.收集服务器信息
主要收集服务器系统版本、IP地址、ARP连接、路由信息、密码信息、历史命令、当前权限、网络连接、进程信息、服务信息、SSH登录信息、环境变量、计划任务等多种信息。

#### 2.目录结构信息收集
主要对服务器上的目录结构进行信息收集，方便查看服务器的结构目录。

#### 3.关键词信息收集
通过在脚本中设置关键字，可以在服务器上搜索包含该关键字的文件，并将该文件所在的目录写入到指定文件中，然后我们可以通过查询该文件来访问指定目录，在配置文件中找到我们所需要的关键信息。


### 二、使用方法
#### 1.查看帮助

<img width="604" alt="image" src="https://user-images.githubusercontent.com/53456907/182522068-67d4d726-289f-44ed-8afe-231b84012d9d.png">


`gather -h`

<img width="659" alt="image" src="https://user-images.githubusercontent.com/53456907/182522018-711c633a-64ed-49ed-afa2-2f115ec78f04.png">


#### 2.常规扫描

`gather -s`

常规扫描主要扫描服务器信息，将结构输出到/tmp/report/result.txt中

<img width="658" alt="image" src="https://user-images.githubusercontent.com/53456907/182521719-9cf35356-b36d-4292-880c-d5d418e5f8db.png">


#### 3.全部扫描(建议使用)

`gather -a`

全部扫描会收集服务器信息、收集服务器目录结构、对关键字进行信息收集，并将结果输出到/tmp/report目录下，会生成tree.txt、result.txt、keyword.txt

<img width="840" alt="image" src="https://user-images.githubusercontent.com/53456907/182523337-09cbaae3-aff0-4802-b381-2126dda68c71.png">


#### 4.结果输出

<img width="481" alt="image" src="https://user-images.githubusercontent.com/53456907/182523470-f86a2e5a-300a-47dd-9d87-cf6d60a00680.png">
