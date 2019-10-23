
# 随便写的东西

## 我也不知道写什么

### 添加文件read.md

#### 符合markdown格式

* 将该文件存储到厂库

* 你说干嘛就干嘛

***sdfasfsa***

~~dsfasfsafasfsaf~~

~~~～～～
(```)
import pymysql
db = pymysql.connect(host='176.122.20.89',
                     port=3306,
                     user='root',
                     password='123456',
                     database='stu',
                     charset='utf8')
cur = db.cursor()
'''
name = input('输入名字:')
sql = "select * from interest where name='%s';"%name
'''
sql = 'select * from class1 where sex=%s and score>%s;'
cur.execute(sql,['m',85])  # 执行语句

all_row = cur.fetchall()
print(all_row)

cur.close()
db.close()

(```)
