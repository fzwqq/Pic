#### Pic Respostory

---

折腾了各种图床,免费的确实是最贵的. 

考虑到个人博客不商用, 最后选择稳定靠谱易管理的github.

> 感谢Github, 感谢MicroSoft, 以下省略3000字

* 外链:= https://raw.githubusercontent.com/fzwqq/Pic/master/ + img_id

---

#### 搭配typora + iCloud Drive食用, 效果较佳:

1. 修改typora 图片保存路径为当前文件夹路径.
2. 自定义一个文件夹,初始化Git仓库.(笔者放在~/iCloud/Pic) 
3. 写个脚本(节省时间:) _Pic.sh

```shell
#_Pic.sh 
mv *.png ~/iCloud/Pic
cd ~/iCloud/Pic
git add .
git commit -m "upload"
git push Pic master
```

4. 执行 ./_Pic.sh 即可 (初次执行需要先设置权限 chmod 755 _Pic.sh_)