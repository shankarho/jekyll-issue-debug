# jekyll-issue-debug

jekyll-data plugin is current disabled and the site builds fine

To reproduce the issue

* uncomment jekyll-data in en-us-site/_config / plugins
* uncomment jekyll-data in en-us-site/Gemfile
* run command en-us-site/bundle update
* run command en-us-site/bundle exec jekyll build

The above should result in 

'''
Liquid Exception: undefined method `to_liquid' for #<Jekyll::Theme:0x007fbbceb08a10> in assets/css/styles.css
jekyll 3.7.3 | Error:  undefined method `to_liquid' for #<Jekyll::Theme:0x007fbbceb08a10>
'''
