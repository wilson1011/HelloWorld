# HelloWorld
这是我一个Helloworld仓库 


20171230  更改:
1、学习怎么使用gitHub 代码版本托管；
2、学习怎么create pository ;
3、学习怎么create 一个分支 branch；

#如果color中定义了几种颜色区间，都可以分割出来 
for (lower, upper) in man_color:
    print lower
    print upper

    # 创建NumPy数组
    lower = np.array(lower, dtype = "uint8")#颜色下限
    upper = np.array(upper, dtype = "uint8")#颜色上限


    # 根据阈值找到对应颜色
    mask = cv2.inRange(image, lower, upper)
    output = cv2.bitwise_and(image, image, mask = mask)

    # 展示图片
    cv2.imshow("images", np.hstack([image, output]))
    cv2.waitKey(0)













