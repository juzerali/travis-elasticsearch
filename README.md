# travis-elasticsearch


[![](https://secure.travis-ci.org/juzerali/travis-elasticsearch.png)](http://travis-ci.org/#!/juzerali/travis-elasticsearch)

Get a elasticsearch instance running with a one-liner and use it in your tests.


## Usage

```
curl https://raw.github.com/juzerali/travis-elasticsearch/master/travis-elasticsearch.sh | ELASTICSEARCH_VERSION=0.20.2 bash
```

ELASTICSEARCH_VERSION:

You have to specify one of these versions:

- 0.20.2
- 0.20.1
- 0.20.0
- 0.19.11


## Travis-ci

Edit your .travis.yml and use travis-elasticsearch as a *before_script* script. 
For example if you want to use elasticsearch 3.6.1 with the default settings you can add this
line to your .travis.yml: ::

```
before_script: curl https://raw.github.com/juzerali/travis-elasticsearch/master/travis-elasticsearch.sh | ELASTICSEARCH_VERSION=0.20.2 bash
```
