# Intro - 125 words right now

For a long time, cookies were the main way to store information about users visiting your app or website. They were used to record stateful elements like shopping cart items or options changed by a user. They were also used to remember user browsing habits or to keep a user logged in while they went form page to page. Then, HTML5 appeared on the scene and introduced LocalStorage and SessionStorage as unique data storage options. Both of these new objects boasted a much large storage capacity than cookies at a whopping 5MB. But between these three options, which is the best storage for your website? In this article, we will compare and contrast all three in the hopes of making that decision clearer for you.

# Cookies - 150 to 200 words; about 178 words right now

First we'll start by exploring basic information about cookies. We'll also go over some of their pros and cons. So, what are cookies? According to whatarecookies.com they are small text files that are placed on a user's computer by a website. They hold a very small amount of data at a maximum capacity of 4KB, but they are capable of storing different types of information, such as the pages visited on a site or a user's login information. Cookies are limited in that they can only store strings.

Many secure websites employ cookies to validate their users identities after they've logged in to prevent them from having to re-enter their credentials on every page. Another use for cookies is to customize or adjust user experience based on limited browsing history on the site.

# Two types of cookies

There are two types of cookies: persistent cookies and session cookies. Session cookies are ones that do not contain an expiration date. Instead they are stored only as long as the browser or tab is open. As soon as the browser is closed, they are permanently lost. This type of cookie might be used to store a banking user's credentials while they are navigating within their bank's website since their information would be forgotten as soon as the tab is closed.

Persistent cookies do have an expiration date. These cookies are stored on the user's disk until the expiration date and then permanently deleted. They can be used for other activities such as recording a user's habits while on a particular website in order to customize their experience.

https://www.cisco.com/c/en/us/support/docs/security/web-security-appliance/117925-technote-csc-00.html#anc0
--persistent cookies; contains an expiration date
--stored on a disk until the specified expiration date
--before html5 app data was stored in cookies in every server request
--can set the expiration time for each cookie
--stores data that has to be sent back to the server
--smallest space (4KB limit) for name, value, expiry date
--only allow you to store strings

# LocalStorage - 150 to 200 words; about 167 words right now
--stores data with no expiration date
--data is not sent with every HTTP request reducing traffic between client and server
--data persists until explicitly deleted; data saved for all current and future visits; can only be cleared through Javascript
--data stored is only available on same origin
--high storage limit just like session storage (5MB)
--allow you to store js primitives/objects
--improvement on cookies
--good for data that needs to be stored for longer periods of time
--an example of a good way to use LocalStorage would be in an application that may be used in regions without a persistent internet connection; the threat level of the data stored in this situation would have to be very low; to protect client privacy, it would be good to upload the data when connection is reestablished and then delete the locally stored version
--another option is to encrypt data in local storage
--firms with data that must be secured would not allow use of LocalStorage for their clients

# SessionStorage - 150 to 200 words; about 90 words right now
--stores data only during session; changes made are saved for current and future visits within the same window, i.e. until the browser or tab is closed
--data stored is only available on same origin
--data is not transferred to the server
--storage limit is medium; larger than cookie, but smaller than LocalStorage (5MB)
--allow you to store js primitives/objects
--good for information that is session specific
--with the presence of dynamic ajax-driven interfaces this can be used to restore a specific site to the way that they last experienced it


# Conclusion - 100 words
--
