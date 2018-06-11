- `赋值` var=value
- `相等` var = value 
- `查看PID` pgrep gedit 
- `替换` cat /proc/12501/environ | tr '\0' '\n'
- `引用变量` echo $var 或者 echo ${var}
- `获取长度` echo ${#var}
- `临时变量` HTTP_PROXY=http://192.168.0.2:3128 export HTTP_PROXY 
- `环境变量` $PATH
- `增加环境变量` export PATH="$PATH:/home/user/bin"
- `$PATH通常定义在` /etc/environment | /etc/profile | ~/.bashrc
- `常用环境变量`：HOME PWD USER UID SHELL PS1
- `判断是否超级用户`
```sh
if [$UID -ne 0];then
echo Non root user. Please run as root
else 
echo "Root user"
fi
``` 
- `输出颜色文字`
```sh
echo  "\e[1;42mI love you,赵丹\e[0m这里是天堂!"  #背景
echo "\033[37;31;;5mMySQL Server Stop...\033[39;49;0m" # 闪烁
echo -e "\033[37;31;1mMySQL Server Stop...\033[39;49;0m" # 加粗
echo -e "\033[37;31;4mMySQL Server Stop...\033[39;49;0m" # 下划线
echo -e "\033[37;31;7mMySQL Server Stop...\033[39;49;0m" # 反显
echo -e "\033[37;31;8mMySQL Server Stop...\033[39;49;0m" # 隐匿
```
**参考连接**

- [ubuntu系统修改终端提示符及设置颜色高亮
](http://www.cnblogs.com/Norlan/p/4944861.html)
- [注释](https://www.jb51.net/article/52377.htm)

