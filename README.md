# Pyomic - 高维交互式绘图网站

![Logo](https://github.com/Jae0v0/img_folder/blob/main/162262901949367.png)

[![docs](https://img.shields.io/badge/docs-passing-brightgreen.svg)](https://github.com/Starlitnightly/Pyomic)

Pyomic是一种轻量级交互式可视化工具，可帮助研究人员使用平行图和其他图形方式来表示信息，从而发现高维数据中的相关性和模式。

## 可用功能
功能栏在网页上方，可以根据需求进行滚动
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/5.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)


滚动之后，点击相应模块会用蓝色标注选中，并调用相关功能
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/4.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)


具体功能与pyomic库相似
| 功能    | 描述 |
| ---------------- | ------------ |
| Trans_corr_matrix | 计算相关相邻矩阵（直接和间接）（无标度网络） |
|Select_module	| 从相关相邻矩阵中选择基因模块 |
|Analysis_cocharacter	| 计算基因和性状相关矩阵 |
|Find_DEG	|筛选差异表达的基因/蛋白质 |
|ID_mapping	|探头匹配转换 |
|Enrichment_KEGG	| KEGG基因富集分析 |
|Enrichment_GO	| GO基因富集分析 |
|Enrichment_GSEA	|基因集富集分析 |
|Plot_GSEA	|绘制GSEA的结果图 |
|Plot_gene_expression	|在矩阵中绘制目标基因表达 |
|Density_norm | 消除样品批次效应，数据归一化 |
|ID_mapping | 通用探针匹配转换基因 ID |

Pyomic有两种模式
- 网络服务器模式（如果您的数据是 CSV）
- 在 jupyter notebook（用于可视化 Python 数据），[详细内容点击此处](https://github.com/Starlitnightly/Pyomic)

## 详细使用
Find_DEG提供图片显示和数据下载
```javascript
在界面下方可以键入csv文件或直接上传csv文件，实现在线编辑功能
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/2.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)
```javascript
点击“导出JSON”打包可编辑excel表格数据给后端调用函数，返回需要图片返回到前端
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/1.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)
```javascript
点击放大镜图标可以放大图片
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/6.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)
```javascript
有的函数还会返回数据到可编辑excel表格中，提供下载功能
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/7.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)


ID_mapping单提供数据下载，无图片接口
```javascript
上传需要csv文件
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/8.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)
```javascript
下载匹配转换生成的数据
```
![在这里插入图片描述](https://github.com/Jae0v0/img_folder/blob/main/9.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80Mzk1MDY0Mw==,size_16,color_FFFFFF,t_70#pic_center)



## 如何搭建环境
前端(vue搭建)运行：
```javascript
npm install
npm run serve
```
后端(django搭建)运行：
```javascript
python manage.py start
```
