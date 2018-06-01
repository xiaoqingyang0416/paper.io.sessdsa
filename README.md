# paper.io.sessdsa
地空数算课2018期末作业：纸带圈地

【北京大学地空学院数据结构与算法课程实习作业2018】

【陈斌 gischen(at)pku.edu.cn】

课程网站：[【数据结构与算法Python版】](http://gis4g.pku.edu.cn/course/pythonds)

## 比赛参数公告
### __建议先用棋盘大小102*101（k=51,h=101)，每局2000个回合，每局时限30秒__

上述参数在热身赛之后可能会根据赛情调整。

## 文件说明
- README.md：本文件
- LICENSE：授权文件GPL 3.0
- UPDATE.py：更新工具
* match_core.py：游戏执行逻辑（配套代码分析报告）
* match_interface.py：游戏逻辑接口
- sessdsa2018-paper.io.pdf：实习作业说明PPT
- paper_io_20180522.pdf：说明文档
- AI_Template.py：AI编写模板（配套说明pdf文件）
- [AI]：一些示例AI
* visualize_console.py：控制台复盘代码（配套说明md文件）
* roundRobin.py：循环赛代码
* solo.py：自定义比赛与记录回放工具
* glory_of_mankind.py：人机对战工具

## 修改历史

### 20180601
- 参数接口更改
    - 参数内容更改
        - stat现包括场地大小与比赛记录
        - storage改为多局比赛间不重置的私有存储
        - 原场地信息stat现为stat\['now'\]
        - 原场地大小storage\['size'\]现为stat\['size'\]
        - 原比赛记录storage\['log'\]现为stat\['log'\]
    - AI函数接口更改
        - load与summary函数增加比赛信息stat接收，详见AI_Template.pdf
- match_core.py中移除match_with_log函数
- 陈天翔创建游戏逻辑接口代码match_interface.py，增加多局对决功能
    - 多局比赛起始、结束函数接口暂定为init与summaryall

### 20180531
- 陈天翔创建人机对战工具

### 20180530
- 陈天翔为比赛可视化工具增加进度条功能

### 20180529
- 陈天翔优化内核log记录方式，并在load函数读入的存储中放置初始场景

### 20180527
- 陈天翔为内核增加对summary函数支持
- 陈天翔为内核增加match.DEBUG_TRACEBACK接口，便于调试

### 20180524
- 陈天翔将自定义比赛工具改为canvas显示，并增加了记录回放功能
- 陈天翔为内核增加帧读取接口
- 陈天翔创建了本地更新工具

### 20180523
- 陈天翔为内核代码增加超时终止功能

### 20180522
- 张赖和创建了期末大作业总说明文档
- 陈天翔创建了比赛工具
- 陈天翔为内核代码增加了load函数接口，并修改了相关代码读取玩家AI的逻辑

### 20180521
- 陈天翔上传了控制台复盘代码，修改了执行逻辑使之支持可变回合数/思考时间，并上传了示例随机游走AI
- 陈天翔更改复盘文件格式（由shelve对象改为pkl格式）与输出路径（保存至log文件夹）
- 张赖和创建了循环赛代码，并上传了另外4个示例AI
- 陈天翔创建了AI模板与配套的说明文件

### 20180520
- 陈天翔上传了游戏执行逻辑

### 20180519
- 陈斌创建了实习作业说明PPT。

### 20180518
- 陈斌创建代码仓库和README.md文件。
