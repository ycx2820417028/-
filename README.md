def draw_heart_shape():
    turtle.speed(1)  # 设置绘制速度
    turtle.color('red')  # 设置颜色
    turtle.begin_fill()  # 开始填充颜色

    # 绘制爱心的上半部分
    turtle.left(50)
    turtle.forward(112)
    turtle.circle(56, 200)
    turtle.right(140)
    turtle.circle(56, 200)
    turtle.forward(112)

    # 绘制爱心的下半部分
    turtle.left(120)
    turtle.circle(-56, 200)
    turtle.right(80)
    turtle.circle(-56, 200)
    turtle.forward(112)

    turtle.end_fill()  # 结束填充颜色

    # 隐藏turtle画笔
    turtle.hideturtle()

# 初始化turtle环境
turtle.setup(width=600, height=400)
draw_heart_shape()

# 点击窗口时关闭
turtle.done()
