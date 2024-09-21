```json
{
"musicId": "2118436701",
  "date": "2024.09.04 21:00",
  "tags": ["python","打包"],
  "description":"试着把python项目打包成exe可执行文件，看到许多推荐使用pyinstaller  但是在打包的时候默认打包执行代码而且不会打包静态文件（如数据库。图片，html文件等）和linux的二进制打包一样 "
}
```

## 起因

### 试着把python项目打包成exe可执行文件，看到许多推荐使用pyinstaller  但是在打包的时候默认打包执行代码而且不会打包静态文件（如数据库。图片，html文件等）和linux的二进制打包一样

其实很简单 我们，执行打包命令的时候把静态文件的目录add 进去
`python  pyinstaller --add-data "templates;templates" your_script.py`


