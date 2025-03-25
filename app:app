from flask import Flask, render_template, url_for, redirect, request

app = Flask(__name__)


@app.route('/', methods=['GET', 'POST'])
def hello_world():  # put application's code here
    return render_template('index.html')



@app.route('/number/<int:num>')
def index():
   return render_template('index.html')


   @app.route('/square', methods=['POST'])
   def square():
       try:
           number = float(request.form['number'])
           result = number ** 2
           return f'The square of {number} is {result}'
       except ValueError:
           return 'Please enter a valid number.'


if __name__ == '__main__':
    app.run()
