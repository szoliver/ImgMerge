# ImgMerge
合并多个图片到一个指定大小的新图片中，并按相同尺寸及顺序排列

#C# DEMO
```c#
Image img1 = Image.FromFile(@"C:\Users\ChenXB\Pictures\hwl.jpg");
Image img2 = Image.FromFile(@"C:\Users\ChenXB\Pictures\sgh.jpg");
Image img3 = Image.FromFile(@"C:\Users\ChenXB\Pictures\syf.jpg");
Image img = OlivetTools.ImgeHandler.ImgMerge(200, 300, 5, null, 
            new Image[] { img1, img2, img3, img2, img3, img2 });
img.Save(@"C:\Users\ChenXB\Pictures\allinone.jpg");
```
