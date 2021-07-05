# HTML & CSS & JAVASCRIPT
## Design and Build Websites 

### Local Storage
#### INTRODUCING HTML5 STORAGE
 ##### HTML5 Storage is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” 

 ##### From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

 #### What is HTML Web Storage?
##### With web storage, web applications can store data locally within the user's browser.

##### Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.

 #### USING HTML5 STORAGE

##### HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

#### TRACKING CHANGES TO THE HTML5 STORAGE AREA

##### If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.

#### HTML Web Storage Objects
##### HTML web storage provides two objects for storing data on the client:

##### `window.localStorage` - stores data with no expiration date
##### `window.sessionStorage` - stores data for one session (data is lost when the browser tab is closed)
