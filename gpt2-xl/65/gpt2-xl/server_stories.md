Once upon a time, there was a server named "pizza." She'd been hacked into by criminals, who took everything the server had saved. They left an incriminating blog with her personal information, and then posted the URL to the world. This, the servers reasoned, would help prove who was really behind the hack. Now the servers run PHP and Javascript and MySQL, and they're so used to seeing the same malicious HTML every month that they'll just throw their hands up and call it a day. But this wasn't happening just for one person. Many other websites, including "pizza" itself, were falling victim to what's known as an XSS (Cross-Site Scripting) attack.

How XSS happens

XSS attacks work like this: the hacker enters an input field, like "some-password." The website accepts it, and your computer sees that code, runs it, gets the password to your account. But this is what happens (in web's case) when you enter "password":

<input type="text" id="some-password">

<input type="password">

<span>I <i>think that's the way it works.</i></span>

And then the server:

<b>HACKED</b>

<b>by the FBI</b>

XSS Attacks Can Be Harder Than You Think

Let's say