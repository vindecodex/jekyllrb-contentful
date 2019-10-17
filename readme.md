### Jekyll with Contentful

###### Requirements
1. Ruby version >= 2.4.0 using rbenv

  `if you have a ruby already install as default then you install using rbenv, to switch from rbenv ruby you can try this code:`

  ```
  export PATH="$HOME/.rbenv/bin:$PATH"
  eval "$(rbenv init -)"
  ```

2. [Jekyll v3.6.3](https://jekyllrb.com)

3. [Contentful](https://contentful.com)

###### Running the applicatoin

1. ```git clone git@github.com:vindecodex/jekyllrb-contentful.git```

2. ```cd jekyllrb-contentful```

3. ```bundle install```

4. ```bundle exec jekyll contentful```

5. ```bundle exec jekyll server```

###### IF want to create new just go to (jekyll)[https://jekyllrb.com]

1. add this to Gemfile

```
group :jekyll_plugins do
  gem "jekyll-contentful-data-import"
end
```

2. add your space id and access token of contentful below plugins:

```
contentful:
  spaces:
    - links:
        space: 6sqgd61ctg5h
        access_token: r1L36G0edffLovcZsWjwOa322u70MxlnqnXJJVukFog
```
