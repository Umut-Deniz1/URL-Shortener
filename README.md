# URL-Shortener

In this app, I used the Hashids library in python. Hashids is a library that generates a short unique ID from integers. There are two steps, first one constructs a hash using the hashes.encode() method, passing it the URL ID; I save the result in a variable called hashid. As an example, the call hashids.encode(3) might result in a unique hash like e5vq depending on the salt you use.

 The second one is that I added a new route that takes the short hash the application generates and decodes the hash into its integer value, which is the original URL’s ID. 
 
 As a result, it will redirect users to the original URL.
 
 ## Installation
Install the dependencies and import libaries
```
pip install flask hashids 
import sqlite3
from hashids import Hashids
from flask import Flask, render_template, request, flash, redirect, url_for
```

## Preview

