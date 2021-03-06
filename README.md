# django-dotenv

[![Build Status](https://travis-ci.org/jpadilla/django-dotenv.svg)](https://travis-ci.org/jpadilla/django-dotenv)
[![PyPI Version](https://pypip.in/version/django-dotenv/badge.svg)](https://pypi.python.org/pypi/django-dotenv)

[foreman](https://github.com/ddollar/foreman) reads from `.env`. `manage.py`
doesn't. Let's fix that.

Tested on Python 2.6, 2.7, 3.2, 3.3, and 3.4.

## Installation

```
pip install django-dotenv
```

## Usage

Pop open `manage.py`. Add:

```
import dotenv
dotenv.read_dotenv()
```

You can also pass `read_dotenv()` an explicit path to the .env file, or to the directory where it lives. It's smart, it'll figure it out.

That's it. Now go 12 factor the crap out of something.
