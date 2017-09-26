`Flask-Migrate文档 <https://flask-migrate.readthedocs.io/en/latest/>`_

步骤：

1. python manage.py db init

2. python manage.py migrate

3. python manage.py db upgrade

第3步加上--sql参数

    python manage.py db upgrade --sql

就不会直接修改数据库, 只显示要执行的sql，有时特别有用
