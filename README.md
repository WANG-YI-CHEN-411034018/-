# 參考自: https://steam.oxxostudio.tw/category/python/ai/ai-mediapipe-gesture.html  
## 使用 MediaPipe 和 OpenCV 進行手勢識別  
* 這個 Python 程式利用了 MediaPipe 和 OpenCV 庫來識別通過網絡攝像頭捕捉到的手勢。該程序檢測手部地標並計算手指之間的角度以識別特定手勢。
* 遇到的困難:
  安裝opencv-python 和 mediapipe後人會有No module named 'cv2'的問題，再命令提示字元在安裝一次後解決，應該是版本換環境問題  
* 工作原理:  
這個程序捕捉來自網絡攝像頭的視頻。  
它使用 MediaPipe 库檢測手部地標。  
根據地標坐標計算手指之間的角度。  
基於角度，識別特定的手勢並在屏幕上顯示。  
此外，特定的手勢會觸發手周圍的馬賽克效果。
*附加說明:  
本程序依賴於手部地標檢測的準確性，這可能會因光線條件和手部位置而變化。  
手勢的識別基於預定義的角度閾值。可能需要調整以在不同環境中獲得更好的性能。  
