
# Introduction
要從width * height * 65的Xray截面圖中還原一頁紙面的文字
方法為從65層的data中判斷每個pixel是否有墨水Ink。
透過這判斷方式。

# Method
- 方法一：訓練model判斷1 x 1 x 65是否有墨水。但墨水判斷可能跟周遭的對比有關。單純的絕對強度可能不夠
- 方法二：訓練model判斷n x m x 65的圖型(n,m 小於width, Height)的正中央的pixel是否有墨水。
- 方法三：訓練model，直接對整個width * height * 65的圖做segmentation。標示出有墨水的範圍

  
# Reference 

https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/overview
