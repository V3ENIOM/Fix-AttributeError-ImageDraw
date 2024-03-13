# Fix AttributeError ImageDraw in Python Crash Course on Coursera.
In this repo, I will discuss how to solve this problem

`AttributeError: 'ImageDraw' object has no attribute 'textbbox'` 

in Python Crash Course on Coursera.

Firstly, this error occurs because of the Word Cloud version.
The `ImageDraw.textsize()` method was deprecated in PIL version 9.2.0 and completely removed beginning with version 10.0.0 on 2023-07-01.

The `ImageDraw.textbbox()` method was introduced in version 8.0.0 as a more robust solution.
So to solve this problem  you must install an old version of it. 

Step 1 : 
Take backup for all commands in the first field, then type
```bash
!pip list
```
to show all packages installed.

**Note: Hit RUN after every command and wait to be executed** 


![](https://i.ibb.co/M8Jvs8g/11.png)


step 2:
uninstall wordcloud & pillow Package
```
!pip uninstall -y wordcloud
!pip uninstall -y pillow
```


![](https://i.ibb.co/ZN74kRt/uni.png)


step 3:

install an old version of WordCloud 
```
!pip install wordcloud==1.8.1
```


![](https://i.ibb.co/1r8r858/in.png)


Step 4 : 

Save the project and choose "Close and Halt" from the file menu 


![](https://i.ibb.co/3Y6kc9M/save.png)


step 5 : 

Reload the page and paste the commands that we took a backup 

Run all commands of the project as usual.


![1](https://i.ibb.co/NKSf9CY/1.png)


.

.

.


![1](https://i.ibb.co/jH4X40X/3.png)
