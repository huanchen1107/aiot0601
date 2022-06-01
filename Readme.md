# AIoT Github



## Lecture 15: IoT Flask Web (deploy to heroku)
###### Author : Huan Chen

### step 0: Setup Environment
* github, heroku account  setup
* download HeidiSQL, VS code
  
### step 1 : Clone this github
* 把local的 \aiot0531.git 殺掉 (產生自己的git管理員) 方便建立新的git repository
* 推送至github 建立新的 aiot0531 https://github.com/huanchen1107/aiot0601
  


### step 2 : install some package
* If you want to test locally, you need to install the following packages. (That is the same thing in the requirements.txt)

```python
pip install gunicorn  Flask==2.0.1 Jinja2==3.0.1 psycopg2 sklearn pandas numpy
```

### step 3: add an heroku postgredb

* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb

### step 4: login to heroku pstgredb using HeidiSQL

#### HeidiSQL setup
![heidi](/img/heidi.png)

#### Postgredb in Herolu
![heidi](/img/postgredbOnHeroku.png)
```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 5: import postgredb (in db/postgre.db)


### step 6: setting db in app.py


```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"

```
### step 7: testing locally by running python app.py


![local server success](img/local_success.png)

### step 8: deploy to github (new private github repositoy)

delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github

### step 10: Complete

Sample link 1:
https://awinlab-aiot.herokuapp.com/

Sample link 2: 
https://aiot0601.herokuapp.com/

### Result: (remote random sensor points)

![remote random](img/remote_random.png)

### Result: (remote after AI prediction)

![remote predict](img/remote_AI.png)

