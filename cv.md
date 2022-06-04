# **PAVEL LAPCHENKO**

**Contacts**
==============

**country**: *Belarus*

**city**: *Mogilev*

**e-mail**: *flangerbox@gmail.com*

**About me**
==============

> I am a beginner developer. I am 35 years old. Imu higher engineering education in the field of construction. After graduating from the university, he worked in his specialty in various positions. Currently, I work as a project manager in the field of construction management. In my free time, I study IT technologies.

**Skills**
===========

* Python
* SQL
* HTML/CSS
* Git

**Code example**
================
```
n = int(input())
m = n
mat = [[0 for i in range(m)] for j in range(n)]
var = 1
count_rigth, count_down, count_left, count_up = 0, 0, 0, 0
if m <= 1:
    for i in range(n):
        mat[i][0] = var
        var += 1
else:
    while var <= n*m:
        # заполение по горизонтали в право
        for i in range(count_rigth, n):
            for j in range(count_rigth, m - count_rigth): 
                if i == count_rigth:
                    mat[i][j] = var
                    var += 1 
        count_rigth += 1
        if var > n*m: break
        # заполнение по вертикали вниз
        for j in range(count_down, m):
            for i in range(count_down + 1, n - count_down - 1):
                if j == m - 1 - count_down:
                    mat[i][j] = var
                    var += 1
        count_down += 1
        if var > n*m: break
        # заполнение по горизонтали влево
        for i in range(count_left, n):
            for j in range(m - count_left - 1, count_left, -1):
                if i == n - 1 - count_left:
                    mat[i][j] = var
                    var += 1
        count_left += 1
        if var > n*m: break
        # заполнение по вертикали вверх  
        for j in range(count_up, m):
            for i in range(n - 1 - count_up, count_up, -1):
                if j == count_up:
                    mat[i][j] = var
                    var += 1
        count_up += 1
#output
for i in range(n):
    for j in range(m):
        print(mat[i][j], end=' ')
    print()
```
**Experience**
=============
**Education**
=============
* __University__: Belorusian-Russian University, building faculty, civil engineer
* __Courses__:
    + Generation Python - course for beginners (stepik.org)
    + Generation Python - advanced course (stepik.org)
    + Programming on Python (stepik.org)
    + Python: basics and application (stepik.org)