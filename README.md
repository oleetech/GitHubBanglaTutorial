
# Git And Github 

1. কম্পিউটার এ একটি নতুন ফোল্ডার এর মধ্যে একটি html টেম্পলেট তৈরী করি। 

![App Screenshot](https://i.postimg.cc/5NBVWqZs/git1.png)


2. একটা সিম্পল ডিজাইন করি html টেম্পলেট  এ।  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Hello, World!</h1>   
</body>
</html>
```
3. টেমপ্লেটটি দেখতে নিচের মত হবে। 
![App Screenshot](https://i.postimg.cc/Hx9wCN9p/git2.png)

4. এবার আমরা আমাদের ফোল্ডার এর মধ্যে গিট সেটআপ করবো। এই ফোল্ডার এ gitbash ওপেন করি। 
![App Screenshot](https://i.postimg.cc/kgZ3x18X/git3.png)

### গিট্ কনফিগার করা : প্রথমে গিট্ কনফিগার করতে হবে।
***প্রথমবার কম্পিউটার এ গিট নিয়ে কাজ করার জন্য গিট কনফিগার করে নিতে হয়।  এটা একবার করলেই হয়.***

git config –global user.name “olee “

git config –global user.email “olee.techs@gmail.com”

5. নিচের তিনটি কমান্ড এক এক করে রান করি। 
```bash
 git init
 git add .
 git commit -m "Create A Html Template"
 ```
 প্রথম কমান্ড : git init  : দ্বারা প্রথমে এই ফোল্ডার কে গিট এর অধীনে নিয়ে আসলাম। 

দ্বিতীয় কমান্ড : git add . : এই ফোল্ডার এর মধ্যে থাকা সমস্ত ফাইলকে গিট এ যোগ করলাম। 

তৃতীয় কমান্ড : কোন একটা কাজ শেষে সেটার আইডেন্টিফায়ার হিসাবে মেসেজ  সেট করলাম । 

6. github এ একাউন্ট না থাকলে github এ  একাউন্ট খুলে লগইন করবো। 


![App Screenshot](https://i.postimg.cc/XJgyGyh3/git4.png)

7. new বাটনে ক্লিক করে একটি repository এর নাম দিয়ে একটি নতুন repository  তৈরী করি। 

মনেকরি এই আমরা এখানে একটি পোর্টফোলিও টেম্পলেট রাখবো তাই রিপোজিটরি এর নাম OleePortfolio রাখলাম। 
create repository বাটনে ক্লিক করে রিপোজিটরি  তৈরী করি.
![App Screenshot](https://i.postimg.cc/GpwQvGMs/git5.png)

8. আমাদের কম্পিউটার এ থাকা ফোল্ডার কে গিটহাবের তৈরী করা repository এর সাথে কানেক্ট করি। 
repository  লিংক কপি করি। 

9. কম্পিউটার এ আমাদের টেম্পলেট ফোল্ডার এ গিট bash ওপেন করে রিমোট রিপোসিটোরি টি যোগ করি। 

git remote add origin https://github.com/oleetech/Oleeportfolio.git

https://github.com/oleetech/Oleeportfolio.git এটা হলো রিপোসিটোরি কপি করা রিপোসিটোরি  লিংক। 

![App Screenshot](https://i.postimg.cc/BbP97RFv/git6.png)


10. আমাদের টেম্পলেট ফাইল গুলোকে আমরা গিটহাব এর তৈরীকৃত রিপোসিটোরি তে পাঠিয়ে দেব। গিট bash এ কমান্ড লিখি। 

```bash
git push -u origin master
```

11. লগইন করার জন্য user name ও পাসওয়ার্ড এর জন্য দুইটি pop up মেনু ওপেন হবে।  গিটহাব এর user name ও পাসওয়ার্ড দিয়ে এন্টার করি। 
![App Screenshot](https://i.postimg.cc/J4nVFDbF/git7.png)


12. গিটহাব এ আমাদের রিপোসিটোরি টি ওপেন করে দেখি। আমাদের ফাইল গিটহাব রিপোসিটোরি তে আপলোড হয়েছে।  

![App Screenshot](https://i.postimg.cc/fL9jyKnP/git8.png)

# Git এর আসল কাজ :
### গিটহাব থেকে ক্লোন করা। 


আমাদের টেম্পলেট এ অন্য একটা কম্পিউটার থেকে নতুন ফিচার যোগ করার জন্য প্রথমে রিমোট রিপোজিটোরি থেকে রিপোজিটোরি টি ক্লোন করতে হবে। 

```bash
git clone https://github.com/oleetech/Oleeportfolio.git
```

ফোল্ডার সহ কোড গুলো আমাদের অন্য কম্পিউটার এ চলে আসবে। 
![App Screenshot](https://i.postimg.cc/hvQqvhKs/git9.png)

### নতুন ফিচার যোগ করা। 
আমাদের টেম্পলেট টি পরিপূর্ন করতে css ,javascript ,images ,fonts  ইত্যাদি ফাইল লাগবে এজন্য আমরা  ক্লোন করা portfolio ফোল্ডার এর মধ্যে css ,javascript ,images ,fonts ফোল্ডার তৈরী করি। 


![App Screenshot](https://i.postimg.cc/y8cc9Tf4/git10png.png)


style.css  ও custom.js নামে css ও js ফোল্ডার এ ফাইল তৈরী করি।  

***নতুন ফাইল গুলোকে গিট এ অ্যাড করি।*** 

যতক্ষণ পর্যন্ত নতুন কোন ফাইল তৈরী হবে গিট নতুন করে কোনো কিছু যোগ করবে না।  আমরা যদি শুধু ফোল্ডার বানিয়ে git add . দেই তাহলে গিট সেটা ট্রেস করা শুরু করবে না যখন কোনো নতুন ফাইল তৈরী করে git add .  করবো তখন গিট ট্রেস করা শুরু করবে। 

```bash
commit -m 'add css and js'
```

***নতুন ফিচার ফাইল গুলোকে  গিটহাব এ সহ পুশ করি।***
```bash
git push
```
**user name ও পাসওয়ার্ড এর জন্য দুইটি pop up মেনু ওপেন হবে।  গিটহাব এর user name ও পাসওয়ার্ড দিয়ে এন্টার করি**

![App Screenshot](https://i.postimg.cc/fbtBSd66/git11png.png)

 ### নতুন ফিচার যোগ করতে কি কোড লিখতে হয়েছে তা দেখা। 

 আমরা একটু আগে নতুন ফিচার যোগ করার পর ফিচার এর নাম আইডেন্টিফায়ার করার জন্য একটা মেসেজ লিখেছিলাম 
 commit -m 'add css and js'

গিটহাব এ ওই commit মেসেজ এ ক্লিক করলে আমরা নতুন ফিচার যোগ করার জন্য কি করেছি তা জানা যাবে। 


![App Screenshot](https://i.postimg.cc/bYCDW5G9/git12png.png)

ক্লিক করলে নিচের মত দেখতে পাবো 


![App Screenshot](https://i.postimg.cc/d18MdpbP/git13png.png)



***এখানে বলা হয়েছে :****

*২ টা ফাইল পরিবর্তন হয়েছে*

*আগের ফাইলে কোনো কিছু যোগ করা হয় নি।* 

*আগের ফাইলে কোনো কিছু ডিলেট করা হয়নি*

*কোনো কিছু নতুন যোগ করলে তা সবুজ আইকন দ্বারা দেখানো হয়।*

#### কি কি পরিবর্তন হয়েছে তা দেখা 
মনে করি আমরা কোন একটা টেম্পলেট এ bootstrap সাপোর্ট অ্যাড করতে চাচ্ছি তাহলে আমাদের index.html  ফাইলে বুটস্ট্র্যাপ অ্যাড করে গিট 

**index.html**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    <title>Document</title>
</head>
<body>
    <h1>Hi I Am Gsm Ashik </h1>   
</body>
</html>
```

 নতুন একটি ফাইল তৈরী করে কমিট করে গিটহাব এ পুশ করি। 
```bash
git add .
git commit -m 'add bootstrap support'
git push
```

পরিবর্তন গুলো দেখতে পারবো কমিটি মেসেজ এ ক্লিক করে। 
![App Screenshot](https://i.postimg.cc/tJHWBSBH/git14png.png)


## Host the website on GitHub:


Go to your GitHub repository and click on the "Settings" tab. 

Scroll down to the "GitHub Pages" section and select "master branch" as your source. Then, click the "Save" button.

if need custom domain write anyrging 

Access the website:
Your website should now be live and accessible at https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/.

Our Web Site Like This 
https://oleetech.github.io/Oleeportfolio/
***click your repository***










