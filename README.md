Задание 1

Найдите ошибку в коде:

```python
from flask import Flask


app = Flask(__name__)


@app.route('') # должен стоять '/'
def home():
   return 'Hello, World!'


if __name__ == '__main__':
   app.run()
  ```

Задание 2.

```python
from flask import Flask

app = Flask(__name__)


@app.route('/')
def home():
    return 'Hello, World!'


@app.route('/user/<username>')
def show_user_profile(username):
    return f'User {username}'


if __name__ == '__main__':
    app.run(debug=True)

```
