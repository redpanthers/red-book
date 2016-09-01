---
sectionid: api-wrappers
sectionclass: h2
title: Writing API Wrappers
is-parent: true
parent-id: ror
number: 5015
---

Code interacting with 3rd party API or scrapping 3rd party website should be placed in the `lib` folder.

How the contents of file should be arranged

```rb
# A scraper to scrpe Alexa ranks

require 'nokogiri'
require 'open-uri'
module Alexa
  # All the constants should be declared on top
  URL = 'http://alexa.com/siteinfo/'
  API_KEY = ENV['API_KEY'] # Place any key if required

  #Alexa.fetch_rank(domain: 'redpanthers.co')
  def self.fetch_rank domain:
    # write the code to fetch results
  end
end
```

Note:

* Always pass the arguments as keyword arguments.
* There should be no direct communication to the DB from the lib folder
* Always return the contents in the format required to be inserted into DB (as a hash)
* Do not include and use the module directly, all the module through self as it would be more redable