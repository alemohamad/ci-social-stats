# CodeIgniter Library: Count URL shares

**ci-social-stats**

## About this library

This CodeIgniter's Library is used to get the count of shares of an URL from social networks (Twitter, Facebook and Google+).  
Its usage is recommended for CodeIgniter 2 or greater.  

*Note:* I recommend that you cache the result, so you won't exceed the limit of requests to each of the social networks. Ideally, do a query every 10 minutes or so.

## Usage

```php
$this->load->library('socialstats');

$url = 'http://github.com';

$tw_shares = $this->socialstats->get_tweets($url);
$fb_shares = $this->socialstats->get_shares($url);
$gp_shares = $this->socialstats->get_plusones($url);
```

![Ale Mohamad](http://codeigniter.alemohamad.com/images/logo2012am.png)
