###### Mon Mar 13 16:44:40 CST 2023


%%%  bowang1988@163.com    2023.3.13 BoWang (School of Automation, HDU)

## 国家自然科学基金结题报告latex模板工程-（非官方模板，不承担任何后果，谨慎使用）

此项目旨在帮助各位老师方便用latex完成基金结题报告的撰写。非官方模板，使用后果自负！！！

不得将本模版用于任何商用用途！！！

模板允许根据个人需要做任意修改，但如果是修改后传播则需要注明基于本工程项目（需标明此工程github地址及作者联系方式）！！！

### 工程说明
系统文件（勿删）：nsfc-report.cls文件完成格式配置；nsfc-report.cfg文件保存项目书各节内容；nsfc-report.bst参考文献格式；latexmkrc用于使用latexmk快速编译。

文件夹：pics存储图片、contents存放基金内容、refs用于放参考文献。

本工程正文固定行距22磅，参考文献间距做了适当压缩

### 文档编译
编译文档请使用XeLaTeX引擎。模版提供latexmk设置文件用于自动编译。将命令行工作目录切换到项目文件夹下，执行
latexmk main-thesis.tex

命令即可自动调用相关程序进行编译，处理各种文件依赖并自动预览。执行`latexmk -c`命令清理所有缓存文件。
手动编译的话 
xelatex main-thesis.tex
命令即可，若文档内部有交叉引用或录入参考文献则需要编译两次。

使用BibTeX录入参考文献需要先运行一次xelatex，运行一次bibtex，再运行两次xelatex。完成编译需运行以下命令：
xelatex bibtex xelatex xelatex

