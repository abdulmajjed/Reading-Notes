# Local Storage.
# DIVING IN.
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet unless your entire web application is served over SSL
3. Cookies are limited to about 4 KB of data — enough to slow down your application see above, but not enough to be terribly useful

SO WE WANT A LOT OF >>>
1. a lot of storage space
2. on the client
3. that persists beyond a page refresh
4. and isn’t transmitted to the server

-------------------
# A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5.
1. In the beginning USER DATA.
2. In 2002Flash cookies.
3. In 2007 Gears.
4. Older versions of Firefox and HTML5.
-------------------
# INTRODUCING HTML5 STORAGE.
1. Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.
-------------------
# USING HTML5 STORAGE
1. HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt or parseFloat to coerce your retrieved data into the expected JavaScript datatype.
2. Calling setItem with a named key that already exists will silently overwrite the previous value. Calling getItem with a non-existent key will return null rather than throw an exception.
3. There are also methods for removing the value for a given named key, and clearing the entire storage area that is, deleting all the keys and values at once.
4. Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index to get the name of each key.
-------------------
# TRACKING CHANGES TO THE HTML5 STORAGE AREA.
1. If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem, removeItem, or clear is called and actually changes something. For example, if you set an item to its existing value or call clear when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.
# STORAGEEVENT OBJECT
1. key	string	the-- named key that was added, removed, or modified
2. oldValue	any--	the previous value now overwritten, or null if a new item was added
3. newValue	any--	the new value, or null if an item was removed
4. url*	string	the-- page which called a method that triggered this change
-------------------
# LIMITATIONS IN CURRENT BROWSERS
--
# HTML5 STORAGE IN ACTION
--
# BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
--
# FURTHER READING

