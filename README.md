# Pyomic - 高维交互式绘图网站

![Logo](https://github.com/Jae0v0/img_folder/blob/main/162259747312723.png)

[![docs](https://img.shields.io/badge/docs-passing-brightgreen.svg)](https://github.com/Starlitnightly/Pyomic)

Pyomic是一种轻量级交互式可视化工具，可帮助研究人员使用平行图和其他图形方式来表示信息，从而发现高维数据中的相关性和模式。

## 可用功能

| 功能    | 描述 |
| ---------------- | ------------ |
| Trans_corr_matrix | Calculate the correlation adjacent matrix (direct and indirect) (scale-free network) |
|Select_module	|Select gene module from correlation adjacent matrix |
|Analysis_cocharacter	|Calculate gene and trait correlation matrix |
|Find_DEG	|Screening Differentially expressed genes/proteins |
|ID_mapping	|Probe matching conversion |
|Enrichment_KEGG	|Gene enrichment analysis of KEGG |
|Enrichment_GO	|Gene enrichment analysis of GO |
|Enrichment_GSEA	|Gene Set Enrichment Analysis |
|Plot_GSEA	|绘制GSEA的结果图 |
|Plot_gene_expression	|在矩阵中绘制目标基因表达 |
|Density_norm | The batch effect of samples was eliminated and the data was normalized |
|ID_mapping | Universal probe matching conversion gene ID |

Pyomic有两种模式
- 网络服务器模式（如果您的数据是 CSV）
- 在 jupyter notebook（用于可视化 Python 数据），[详细内容点击此处](https://github.com/Starlitnightly/Pyomic)

#详细使用
键入csv文件或直接上传csv文件，可在线编辑

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
