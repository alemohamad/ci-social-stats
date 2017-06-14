# CodeIgniter Library: Count URL shares

**ci-social-stats**

## About this library

This CodeIgniter's Library is used to get the count of shares of an URL from social networks (Twitter, Facebook, Google+, Pinterest, LinkedIn and StumbleUpon).  
Its usage is recommended for CodeIgniter 2 or greater.  

*Note:* I recommend that you cache the results, so you won't exceed the limit of requests to each of the social networks. Ideally, do a query every 10 minutes or so.

## Usage

```php
$this->load->library('SocialStats');

$url = 'http://github.com';

$twitter_shares     = $this->socialstats->get_tweets($url);
$facebook_shares    = $this->socialstats->get_fb_shares($url);
$googleplus_shares  = $this->socialstats->get_plusones($url);
$pinterest_shares   = $this->socialstats->get_pins($url);
$linkedin_shares    = $this->socialstats->get_in_shares($url);
$stumbleupon_shares = $this->socialstats->get_stumble_views($url);
$tumblr_shares      = $this->socialstats->get_tumblr_shares($url);
```

![Ale Mohamad](http://codeigniter.alemohamad.com/images/logo2012am.png)
