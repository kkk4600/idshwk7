将图像用傅里叶变换到频域，将水印图像编码，两者运算后进行傅里叶逆变换生成水印图像。图像的能量主要集中在低频部分，高频信息是图像的细节，盲水印叠加在图像的高频区域所有不易被察觉。
这里，oripic.png是原始图像，57117235lina.png是水印图像，隐藏水印后生成test.png，恢复后的水印为shuiyin.png。
使用命令encode.py --image oripic.png --watermark 57117235lina.png --result test.png进行隐藏。
使用使用decode.py --original oripic.png --image test.png --result shuiyin.png恢复水印。
