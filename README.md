# HumanManagerBattle
  Python实现人机象棋对战,数据分析python +Tenstensorflow
  第一次部署项目到git仓库
  第一步完成项目时间规划
  每晚22：00定时推到github上
  
  师兄交流要点：
	多人VR服务器的设计：基于unity c#
		设备：HTC VIVE
		用到的插件 steamVR  VRTK 
  黄老师要求：做一个中国象棋的人机对弈，用python+tensorflow环境，机器学习
  象棋规则及界面实现步骤：
	1.绘制棋盘
	2.绘制棋子
	3.绘制带棋子的棋盘
	4.走棋规则
	5.吃子规则
	6.走棋
	7.判断是否赢棋
	8.按键功能
	9.美化
	10.音效

	
  学习pygame库的使用
  注册下载pygame 
	  py -m pip install -U pygame --user
  演示pygame自带demo
	  py -m pygame.examples.aliens
  查看当前机器支持的显示模式：
	  pygame.display.list_modes()
  全屏显示：
  screen = pygame.display.set_mode((640, 480), FULLSCREEN, 32)
  可变尺寸的显示：
  screen = pygame.display.set_mode((640, 480), RESIZABLE, 32)
  其他、复合模式：
  screen = pygame.display.set_mode((640, 480), HWSURFACE | FULLSCREEN, 32)
  查看当前系统支持的所有字体
  pygame.font.get_fonts()

  font 使用步骤：
  my_font = pygame.font.SysFont("arial", 16)	 字体名 大小
  text_surface = my_font.render("Pygame is cool!", True, (0,0,0), (255, 255, 255))  文字 是否开启锯齿 字体颜色 背

  
  
  学习pygame Vector向量的知识：
  python2.x 使用gameobjects
  python3.x 使用https://www.pygame.org/wiki/2DVectorClass
  
 2019/4/18学习任务 继续学习pygame（10）  修改论文 开始制作答辩ppt
  键盘事件：
   pressed_keys = pygame.key.get_pressed()
    if pressed_keys[K_SPACE]:
        # Space key has been pressed
        fire()

 2019/4/22 修改毕设，论文
 
 ###在廖雪峰的网站学习了海龟绘图
 发现利用turtle画棋盘更方便
 海龟绘图

 在1966年，Seymour Papert和Wally Feurzig发明了一种专门给儿童学习编程的语言——LOGO语言，它的特色就是通过编程指挥一个小海龟（turtle）在屏幕上绘图。
 海龟绘图（Turtle Graphics）后来被移植到各种高级语言中，Python内置了turtle库，基本上100%复制了原始的Turtle Graphics的所有功能。
 开始学习turtle库，掌握其基本用法
 
 
 ###pyinstaller使用方法
	pip install pyinstaller
	#生成单一的exe文件：
		pyinstaller -F test.py
	#基本使用方法：
		pyinstaller -F -i tb2.ico -w 翻译.py
 ###tkinerGUI编程基本使用方法：
	Tkinter 是 Python 的标准 GUI 库。Python 使用 Tkinter 可以快速的创建 GUI 应用程序
	import tkinter
	
	top = tkinter.Tk()
	# 进入消息循环
	top.mainloop()
2019/4/28 论文修改  去重