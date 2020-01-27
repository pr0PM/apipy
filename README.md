# TODO: 
Give that ugly JSON a web UI

# USER GUIDE

###  This maybe a resful API gotta study more about that ;)
  
This is a complete web-app in python3 venv,
with batteries included i.e you mustn't need anything more to run this.

Just clone the repo and run it.

*More to be added to this part !!!*

# How to use the API 

You can use the following http requsts for following operations
 - GET /ai-quote : To get a random quote
 - POST /ai-quotes/<int:id> : To post a new quote in JSON format (Format given below) at given id
 - PUT  /ai-quotes/<int:id> : To edit a quote at the given id

#### JSON format to POST, PUT request
```
{
"id": int,
"author": "author_name"
"quote": "Your author's quote"
}
```

## Using CURL
##### To Get response

curl -X GET http://pr0pm.pythonanywhere.com

##### To Post a quote

curl -H "Content-Type: application/json" -X POST -d '{"id":"intID","author":"author_name","quote":"Q U O T E"}' http://pr0pm.pythonanywhere.com/ai-quotes/intID

##### To PUT/edit a quote
Follow the same method as above

## Using reqbin.com
Hey they've got a nice UI try yourself :P
