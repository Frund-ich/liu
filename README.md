# #控制鼠标键盘
#截图 显示
import pyautogui
from PIL import ImageGrab
import cv2 as cv
#pyautogui.moveTo(100,100,duration=1) 
print(pyautogui.position()) 
#
pyautogui.click(661,1035) 
pyautogui.click(616,475) 
print(pyautogui.size()) 
pyautogui.press('backspace') 

im= ImageGrab.grab(bbox=(1,100,614,297))# 截图 参数为指定区域 
im.save("11.jpg")
src= cv.imread("11.jpg")
print(type(src))
'''cv.namedWindow("input",cv.WINDOW_AUTOSIZE)
cv.imshow("input",src)
cv.imshow("input",src)
cv.waitKey(0)'''
