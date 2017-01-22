# -*- coding: UTF-8 -*-
'''
Created on 2013年06月07日 14时
@description：批量打开win下的应用程序，解决每天开机需要开启很多应用软件；用了这个小工具，可以用她开启应用的这段时间来打杯水或者上个厕所 呵呵
@author: guoff
'''
import os
import time
def WordDay():
  print '今天是工作日，好好工作哦!' # block belonging to the function
  workList =['C:\Users\Administrator\Desktop\Someone.mp3',
    'C:\Program Files\Quest Software\Toad for Oracle\TOAD.exe',
    'E:\工作相关软件\SecureCRT-v6.12.0H\SecureCRT\SecureCRT.exe',
    'C:\Program Files\Tencent\TM\Bin\TM.exe',
    'F:\work\日记备份\eDiary-3.3\eDiary.exe'
    ]
  for i in workList:
    os.system('cmd /c start "" "'+i+'" ')
 
def unWordDay():
  print '今天是自由日，自由发挥好好学习哦!' # block belonging to the function
  stuList =['C:\Users\Administrator\Desktop\Someone.mp3',
    'C:\Program Files\Evernote\Evernote\Evernote.exe',
    #'C:\Program Files\JetBrains\PyCharm\bin\pycharm.exe',
    'F:\书\python\Django_book_2_中文版.pdf',
    ]
  for i in stuList:
    os.system('cmd /c start "" "'+i+'" ')
 
def main():
  week = int(time.strftime('%w',time.localtime(time.time())))
  Hour = int(time.strftime('%H',time.localtime(time.time())))
  print 'week',week,'Hour',Hour
  if week not in [6,0] and (Hour>=8 and Hour<=10):
    WordDay()
  else:
    unWordDay()
main()
