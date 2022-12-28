本仓库作为旧版本原始调度的存放区，需要可自提。 最新调度已集成在FEMIND APP内，欢迎访问我们的官网获取： 511i.cn

铁人司机 2022年12月27日


# helio-x20-interactive-sched

***调度是智力成果，本代码虽然开源，但是请在转载、修改和传播的时候标注出处，支持原创，维护铁人调度良性发展，支持作者不断开发安卓，请不要做无聊的搬运工，谢谢！***

***公告：2.5夏季一键710冷却版已经发布，使用方法和2.0通用教程有所区别，请务必注意！谢谢！并且今后一律采用版本号＋shced＋模式＋（特殊备注）+帧率.sh的方式命名。为避免被重命名，一律使用英文命名，40为省电，45为平衡，60为游戏。望知晓，谢谢！***

***2.5是专为降温而制作，因此会比2.4稍有卡顿，核心响应也没有2.4积极，如果无法忍受，请切换回2.4，2.4是目前综合方面最优秀的调度。另外2.5只有gaming可以打游戏，其他两个打游戏会性能严重不足，甚至发热异常死机，是为夏天远途无法及时充电的外出人士制作的。请合理使用，谢谢！***

2.5 cool冷却版测试结果报告：  
测试机型：360 N4 1503-A01 X20    
一、  
    测试调度：2.5 X20省电冷却版  
    测试结果：  
        温度：32℃   鲁大师跑分：85140  

二、    
    测试调度：2.5 X20平衡冷却版  
    测试结果：  
        温度：34℃   鲁大师跑分：89480  

三、    
    测试调度：2.5 X20游戏冷却版  
    测试结果：  
        温度：36℃   鲁大师跑分：119551  

四、测试时间：3:00-5:09 消耗电量：71→36 平均能耗：35%/小时→3.42分钟/1%电量     

2.5 cool冷却版特殊步骤：  

    1、请在2.0通用教程执行之前，一定要root，并给mt管理器root权限，然后用mt管理器进入/system目录，编辑build.prop文件，用mt管理器在build.prop内搜索"perfserv"定位到里面的"ro.mtk_perfservice_support=1"这行，将1改成0，保存退出。    
    2、如果遇到保存失败的情况，请检查root，如果仍然失败，可以尝试先把build.prop复制到内部存储，修改完再覆盖回去原路径下。  

***备用教程!!!：（如果Tasker执行失败请切换此教程）***  
    1、试试用mt管理器执行，看看代码结果，如果是在七八十行左右出错，就是成功，如果从第一行开始，就是失败。  
    2、如果上面的办法失败，进入这一步：  
    备用步骤：  
    1、在最外面的那一页点击clone or download下载我的仓库文件夹并解压，获得脚本文件。    
    2、将第一步解压得到的脚本文件打开，复制里面全部的内容。  
    3、打开终端模拟器，点击右上角首选项，找到“初始命令”，点击，将第二部复制的代码粘贴进去，确认，保存，划掉后台。  
    4、下次点击终端模拟器直接执行。  
    5、按照以上操作，在需要切换模式的时候复制进入响应代码，操作2~3步即可。  

2.0以上版本通用文字教程：

一、准备并安装软件：tasker（最新版）,supersu,root explorer或者mt管理器,终端模拟器,quickedit

二、具体步骤  
    1、在最外面的那一页点击clone or download下载我的仓库文件夹并解压，获得脚本文件。  
    2、利用root exlporer在/data/app下新建一个脚本，随意命名（例如1.sh），立刻授予权限0777。  
    3、将第一步解压得到的脚本文件打开，复制里面全部的内容，粘贴到第二步新建的脚本文件中（例如1.sh）。  
    4、打开tasker，在任务一栏点击右下角加号，新建任意名称任务，点击√，选择代码→外壳，在命令里输入sh ./data/app/你要的脚本名称（例如sh ./data/app/1.sh），勾选“使用root”，点击返回键，点击左下角的三角形就可以执行，等待几秒上方代码出现绿色小圆点即代表成功执行。  
    5、多按几次返回键退出以保存任务。  
    6、按照以上操作创建省电、平衡、游戏等模式的任务，在需要切换模式的时候进去点击左下角三角即可。  

三、注意事项  
    1、重要的事情说三遍！！！→通知栏显示“无激活的配置文件”没有任何问题！！没有任何问题！！没有任何问题！！不要再问我这个问题了，我们不需要用到这个东西。  
    2、可以设置tasker开机自动执行某个调度，如何操作请百度“tasker创建开机任务”。tasker不需要挂后台，执行成功并保存后就可以划掉后台不管他了。  
    3、重要的事情说三遍！！！系统文件是一次修改成功的，在切换电源管理模式和重启之前一直生效。请勿在高性能模式下运行省电调度，请勿在低电量模式下运行游戏调度！！请勿在高性能模式下运行省电调度，请勿在低电量模式下运行游戏调度！！请勿在高性能模式下运行省电调度，请勿在低电量模式下运行游戏调度！！不要在错误的模式下做错误的事然后反馈跟我说没效果。  

四、内测注意事项  
    1、内测请进QQ群653581517，请遵守群规，文明交流。  
    2、为保证质量，内测反馈请按格式提供资料，请提供：  
        ①有问题的界面和场景的截图或者录屏(一分钟之内)，截图和录屏请务必打开性能监视器、cpuloat之类的能提供cpu、gpu频率和温度的软件。  
        ②详细明了的文字说明和希望达到的预期。  
    3、调度是智力成果，请在转载、修改和传播的时候标注出处，维护铁人调度良性发展。  
    4、铁人调度有特定的格式，不符合者均不是本人亲自编写的调度。  

备注：视频教程跳转链接如下：https://www.bilibili.com/video/av48037831?from=search&seid=17972857981563016449  
视频会不定时更新，敬请关注。  

测试群号：653581517  
POWERED BY 铁人司机    
2019/4/13  5:26
