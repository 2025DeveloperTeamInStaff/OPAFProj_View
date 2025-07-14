# CialloProject_View
AHSFNU创客工坊2025&AHSFNU新媒体部<br>
为新媒体部构建一个云服务，来Make 新媒体部 Great Again<br>
1.对新媒体部大型活动图片视频建立素材库，对同学们开放活动素材的下载<br>
2.实现活动实时拍照返图、实时筛选照片视频等服务
## 1.需求总览
### 1.素材云上传（win、android）
​	1.手机、电脑实时上传某个文件夹里面的图片<br>
​	2.上传到云nas上，云平台进行处理
### 2.素材标签（web）
​	1.（重点)支持现场对上传的图片进行显示、打标签（实时返图）<br>
​	2.素材云上打标签：自动标签时间、活动，支持手动打标签<br>
​	3.收藏、星标图片视频
### 3.在线云平台预览（web）<用户管理>
​	1.自动预览、下载新拍摄的图片及视频，使工作用户进行标签、删除和导出<br>
​	2.手动删除、上传素材<br>
​	3.远程素材库管理<br>
​	4.用户表（包括用户组，临时工作流组）
### 4.临时工作流组
​	对工作流组中现场工作用户上传的素材在线推送到工作流组后勤工作用户，以文件夹形式显示当前工作流中所有的素材<br>
​	一个工作流是独立的，有其指定的名称并将其写入当前工作流的所有素材，直到其结束后将文件归档到云
## 2.项目架构
### 1.前端
​	SpringBoot
### 2.后端
​	Postgresql
### 3.桌面开发
​	.NET
### 4.Android
​	Android
### 5.云存储
​	飞牛存储(主)<br>
​	百度网盘(备份)

## 数据库
 # user
  id username password level token1 token2 token3
 # workflow
   id	name	start_date	last_time	type	<用户列表>
 # res
   //Todo
 # invite
   id	invite_code	from_user	end_date

