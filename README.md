# PwnFunction




open redirects are simple redirects from one web site to another, what could

posible go wrong, you might have seen url like this abc.com/?url=xyz.com 

abc.com redirects xyz.com

Redirection is happen xyz.com as soon as  you vist abc.com (302)


If you happen to change this xyz.com in the url to attacker.com then you will

be redirected to attachers website


why Open redirects


Web site offen requies the redirection all over the place, like after login 

into the website are after even passwd reset


Server side

client site | JS(window.location)
	    | HTML(<meta>) meta tags


Open redirects are security treats | It Depends

Phising

we have check the URL all the time

Some time URL are purly encoded`




Cross-Site-Scripting(XSS)


Same origin policy or simply SOP is a policy that stops one website from 

reading or writing data to another, The policy essentially checks for THREE 

different things in the origin the PROTOCOL, HOST, and PORT only if all the 

THREE are the same for two different Origins then the browser allows

cross-origin read or write for example if we have a website PWNFUNCTION.COM 

another website is STEPFUNCTION.COM then the browser checks if the protocol 

is same in both cases which it is which is HTTP so on to the next check next

it checks for the host obviously they're different one is pwn function  the 

other one's stepfunction so the browser blocks Cross Origin read and write

as you can imagine this is a great feature ensuring some basic web security 

But now let us imagine something like a thought experiment `What if we have 

control over the JavaScript of another website`


`We know that JavaScript has access to HTML documents via the Dom apis which

are provided by browser which means we can manipulate the Dom and make it

look different like defacing a page or something better yet we can steal 

some CSRF tokens which could also be problematic or you can simply read some cookies if you can and send it over to your website via Ajax request

or maybe you form submission

` 

I think you see the picture that I'm trying to paint having access to 

JavaScript
