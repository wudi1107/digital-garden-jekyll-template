---
---


```dataview
table without id ("![|50](" + 图片 + " )") as 图片,
file.link as 书名,
作者 as 作者,
出版社 as 出版社,
出版年 as 出版年,
个人评分 as 评分,
阅读日期 as 阅读日期,
ISBN as ISBN
from #books 
sort 阅读日期
```