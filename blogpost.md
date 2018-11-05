# Intro - 125 words right now

For a long time, cookies were the main way to store information about users visiting your app or website. They were used to record stateful elements like shopping cart items or options changed by a user. They were also used to remember user browsing habits or to keep a user logged in while they went form page to page. Then, HTML5 appeared on the scene and introduced LocalStorage as another data storage option. This new object (along with SessionStorage) boasted a much large storage capacity than cookies at a whopping 5MB. In this article, we will compare and contrast cookies and LocalStorage.

# Cookies - 150 to 200 words; about 265 words right now

First we'll start by exploring basic information about cookies. We'll also go over some of their pros and cons. So, what are cookies? According to whatarecookies.com they are small text files that are placed on a user's computer by a website. They hold a very small amount of data at a maximum capacity of 4KB, but they are capable of storing different types of information, such as the pages visited on a site or a user's login information. Cookies are limited in that they can only store strings.

Many secure websites employ cookies to validate their users identities after they've logged in to prevent them from having to re-enter their credentials on every page. Another use for cookies is to customize or adjust user experience based on limited browsing history on the site.

# Two types of cookies

There are two types of cookies: persistent cookies and session cookies. Session cookies are ones that do not contain an expiration date. Instead they are stored only as long as the browser or tab is open. As soon as the browser is closed, they are permanently lost. This type of cookie might be used to store a banking user's credentials while they are navigating within their bank's website since their information would be forgotten as soon as the tab is closed.

Persistent cookies do have an expiration date. These cookies are stored on the user's disk until the expiration date and then permanently deleted. They can be used for other activities such as recording a user's habits while on a particular website in order to customize their experience.

# LocalStorage - 150 to 200 words; about 167 words right now
After HTML5 came out, many uses of cookies were replaced by the use of LocalStorage. This is because LocalStorage has a lot of advantages over cookies. One of the most important differences is that unlike cookies, data does not have to be sent back and forth with every HTTP request. This reduces the overall traffic between the client and server and reduces the amount of wasted bandwidth. This is because data is stored on the user's local disk and is not destroyed  or cleared by the loss of an internet connection. Additionally, LocalStorage can hold up to 5MB of information. This is a whole lot more than the 4KB than cookies hold.

LocalStorage behaves like persistent cookies in terms of expiration. Data is not automatically destroyed unless it is cleared through Javascript code or unless there is an expiration date set. This can be good for larger bits of data that need to be stored for longer periods of time. Also, with LocalStorage you can not only store strings, but also Javascript primitives and objects.

In my back-end web development course, we discussed cases where LocalStorage would be superior to cookies. An example of a good use of LocalStorage might be in an application used in regions without a persistent internet connection. My course instructor, Dani Roxberry, built such an application and used LocalStorage to protect and store data collected in areas with spotty WiFi or data connections. In order for this to be a good use of LocalStorage, the threat level of the data stored in this situation would have to be very low.  To protect client privacy, it would be good to upload the data when connection is re-established and then delete the locally stored version. Additionally, it would be advantageous to encrypt data that was being stored so that it would not be easily hacked. In our class discussion, we also established that highly vulnerable data, such as financial information, could not be stored or secured properly using LocalStorage in this way.

# Conclusion - 100 words
--
