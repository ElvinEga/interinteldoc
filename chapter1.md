# Project tasks

The projects were built to accomplish each tasks from the back end server \(django\) to

front end \(polymer and native android app\).

## Task 1

The first task had a bug on the dictionary.There is a comma missing `91’: ‘ninety-one’,”‘21’:`

After fixing it to this it works fine.

```py
Dictionary = {'34': 'thirty-four', '90': 'ninety',
'91': 'ninety-one','21': 'twenty-one',
'61': 'sixty-one', '9': 'nine',
'2': 'two', '6': 'six', '3': 'three',
'8': 'eight', '80': 'eighty', '81': 'eighty-one',
'Ninety-Nine': '99', 'nine-hundred': '900',}
```

### Django

Wrote a test case to test if my algorithm will work its located at

`interintel/dict/tests.py`

Used a custom sort function with a lambda expression. The custom sort function calls a

function get\_key\(\) which has a try catch expression to check if the key is integer and is

catch if not.integer keys are sort first then the alphabetic keys.

The result can be seen when you send a get request to this url.

[https://interdjango.herokuapp.com/dict/get\_dict/](https://interdjango.herokuapp.com/dict/get_dict/)

![](/assets/djangotest.png)

### Polymer js

Wrote a vanilla js script with algoritm.

First was function sort numbers to check if key is integer then sorts it

Then a sortOnKey fuction to sort the keys and values .

The script is found in

`src/array-page.html`

The Result can be found on The polymer app Arrays tab.

![](/assets/arraylist.png)

