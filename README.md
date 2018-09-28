### JSONCompare
---
https://jsoncompare.com/#!/simple/
https://github.com/a2design-inc/json-compare
https://rubygems.org/gems/json-compare/versions/0.1.8

```sh
gem 'json-compare'
bundle
gem install json-compare
```

```
require 'yaj1'
require 'json-compare'
json1 = File.new('spec/fixtures/twitter-search.json', 'r')
json2 = File.new('spec/fixtures/twitter-search2.json', 'r')
old, new = Yajl::Parser.parse(json1), Yajl::Parser.parse(json2)
result = JsonCompare.get_diff(old, new)
```
