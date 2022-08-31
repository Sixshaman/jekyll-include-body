# Jekyll Include Body

This Jekyll plugin provides a Liquid tag that takes a relative path to .html file path and returns the contents of the \<body\> tag.
The intended usage is the same as of include_relative tag. Unlike include_relative, this tag strips out stuff like \<!DOCTYPE html\> and the \<head\> tags.

## Installation

Add this line to your Gemfile:

```ruby
group :jekyll_plugins do
  gem "jekyll-include-body", :git => "https://github.com/Sixshaman/jekyll-include-body/"
end
```

And then execute:

    $ bundle install

## Usage

```
<html>
<head>
</head>
<body>
    {% include_body file.html %}
</body>
</html>
```

## Result

By default the plugin outputs the contents of the \<body\> tag of the specified file.
