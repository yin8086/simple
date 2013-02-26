Simple
================
A clone of [Obtvse](http://github.com/NateW/obtvse).

这是一个中文化的[Simple](https://github.com/orf/simple) 版本

About
============
The point of Simple is to be simple. The blog is 1 file (excluding resources) with a few simple pure-python dependancies (Flask, Sqlalchemy, Markdown), it doesn't require a database server, has a small footprint and is fairly fast.

Features
============
* Markdown goodness, no clutter or fuss when writing your posts
* Lightweight and simple
* Supports Disqus comments, Google Analytics and custom fonts (from google's font library)
* Drag and drop uploads
* Includes several Markdown extensions:
    * [CodeHilight](http://pythonhosted.org/Markdown/extensions/code_hilite.html)
    * [Fenced Code Blocks](http://pythonhosted.org/Markdown/extensions/fenced_code_blocks.html)
    * [Table of contents](http://pythonhosted.org/Markdown/extensions/toc.html)

Installation
============
Its quite simple. Go download Python 2.7+, Flask, Sqlalchemy and flask-sqlalchemy and you are good to go.
To create a settings file run create_config.py and enter configuration values when prompted, then run simple.py.

Deployment
============
Deploying Simple is easy. Simply clone this repo (or your own) and install [Gunicorn](http://gunicorn.org/).
Then cd to the directory containing simple.py and run the following command:
``gunicorn -w 4 simple:app``
This will start 4 gunicorn workers serving Simple. You can then use nginx or apache to forward requests to Gunicorn.

Example
============
You can see my blog running this software [here](http://tomforb.es/simple).

中文版运行于[这里](http://pyblog.stardrad.com)

Screenshots
===========
![Admin](http://i1323.photobucket.com/albums/u585/yin8086/00_zps9eaecb09.png)

![Draft](http://i1323.photobucket.com/albums/u585/yin8086/01_zps3c7ea108.png)

![Live](http://i1323.photobucket.com/albums/u585/yin8086/02_zps7afd8c41.png)
