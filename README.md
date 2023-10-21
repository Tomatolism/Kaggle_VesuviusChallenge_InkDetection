
# Introduction
要從width * height * 65的Xray截面圖中還原一頁紙面的文字
方法為從65層的data中判斷每個pixel是否有墨水Ink。
透過這判斷方式。

# Method
方法一：訓練一個model判斷1 x 1 x 65是否有墨水。但墨水判斷可能跟周遭的對比有關。
方法二：訓練一個model判斷n x n x 65的圖型的正中央的pixel是否有墨水

# Reference 

https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/overview
