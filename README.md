# ImgMerge
合并多个图片到一个指定大小的新图片中，并按相同尺寸及顺序排列

#C# DEMO
```c#
Image img1 = Image.FromFile(@"D:\Pictures\hwl.jpg");
Image img2 = Image.FromFile(@"D:\Pictures\sgh.jpg");
Image img3 = Image.FromFile(@"D:\Pictures\syf.jpg");
Image img = OlivetTools.ImgeHandler.ImgMerge(200, 300, 5, null, 
            new Image[] { img1, img2, img3, img2, img3, img2 });
img.Save(@"D:\Pictures\allinone.jpg", System.Drawing.Imaging.ImageFormat.Jpeg);
```
#效果图
（人物图像有经PS处理过）
![image](https://github.com/szoliver/ImgMerge/blob/master/allinone.jpg?raw=true)
