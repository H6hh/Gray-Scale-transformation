# 灰度线性变化 灰度上移、对比度增强、对比度减弱、反色变化    
灰度线性变化 灰度上移、对比度增强、对比度减弱、反色变化  
点运算是指按某种灰度变化系，逐象素地对图像中的每个图像素的灰度值进行变化的方法！![Q$2X8K(UYRXCL 765(YK12F](https://user-images.githubusercontent.com/98206033/227697972-9b465038-f94d-4be0-9a09-89e4be053fd1.png)

一、灰度线性变换  
图像的灰度线性变换是通过建立灰度映射来调整原始图像的灰度，从而改善图像的质量，凸显图像的细节，提高图像的对比度灰度线性变换的计算公式：s=ar+b![A`U T@~6N3TXWS6V9O2I}WR](https://user-images.githubusercontent.com/98206033/227697701-0bd41d9c-fee1-4f0a-9d01-16047f7b2e29.png)
也可以用此公式表示：Db=aDA+b中，DB表示灰度线性变换后的灰度值，DA表示变换前输入图像的灰度值，a和b为线性变换方程的参数，分别表示斜率和截距：
a=1，b=0时，保持；  
a=1，b≠0时，灰度值上移或下移；  
a=-1，b=255时，原始图像灰度值反转（黑变白，白变黑）；  
a＞1时，对比度增强；  
0＜a＜1时，对比度减弱；  
a＜0时，图像求补，暗区变量，亮区变暗。  

二、灰度值上移  
DB=DA+50，DB=DA+100  
通过上移改变，使图像变白，变得更白![duibi1](https://user-images.githubusercontent.com/98206033/227698286-da226d65-6186-4ecb-81dd-bd70a4f6a267.png)
![更白了](https://user-images.githubusercontent.com/98206033/227698294-aa7e0f20-5429-45be-9dd6-bb466f2bd106.png)  
三、对比度增强变换  
DB=DA*1.5  ![对比度增强](https://user-images.githubusercontent.com/98206033/227698669-6a61228d-036b-4dcb-a131-39f7c7fb367f.png)  
四、对比度减弱变换  
DB=DA*0.8  
![对比度减弱](https://user-images.githubusercontent.com/98206033/227698805-c4c79a4a-d6b6-4ccf-af96-fa673bdb35df.png)  
五、反色变换  
又称为求补变换，对原图像像素值进行反转，白色变黑色，黑色变白色的过程  
DB=255-DA  ![反色变换](https://user-images.githubusercontent.com/98206033/227699131-5b1e230f-ea0e-49d6-a026-eadaa60641d8.png)  
医学上的应用，对CT图像反色变换更方便医生查看图像，如图是对乳腺癌病灶的反色变换，黑色更突出病灶！
![乳腺癌病灶](https://user-images.githubusercontent.com/98206033/227699296-a261fb1c-bbf2-4927-b86c-f90125e308cd.png)
