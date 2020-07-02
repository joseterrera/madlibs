To run this app create a virtual environment where you install flask and debugtoolbar:
1. $ python3 -m venv venv
2. $ source venv/bin/activate
 
3. (venv)$ pip3 install flask
4. (venv)$ pip install flask-debugtoolbar
5. (venv) $ flask run or run flask in development mode: 
(venv) $ FLASK_ENV=development flask run


Test class Story on terminal using iphyton:
1. %run stories.py
2. story = Story(
    ["place", "noun", "verb", "adjective", "plural_noun"],
    """Once upon a time in a long-ago {place}, there lived a
       large {adjective} {noun}. It loved to {verb} {plural_noun}.""")

3. story.generate({'place' : 'london', 'noun': 'deer', 'adjective': 'pretty', 'verb':'sail', 'plural_noun': 'animals'})

output: 'Once upon a time in a long-ago london, there lived a\n large pretty deer. It loved to sail animals.'
