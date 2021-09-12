# CRUD

## Status Codes Based On REST Methods

### In your own words, describe what each group of status code represents:

#### - 100’s = The HTTP 100 Continue informational status response code indicates that everything so far is OK and that the client should continue with the request or ignore it if it is already finished

#### - 200’s = This is a list of Hypertext Transfer Protocol (HTTP) response status codes.

#### - 300’s = The data requested actually resides under a different URL, however, the redirection may be altered on occasion (when making links to these kinds of document, the browser should default to using the Udi of the redirection document, but have the option of linking to the final document) as for “Forward”.

#### - 400’s = The request had bad syntax or was inherently impossible to be satisfied

#### - 500’s = The server encountered an unexpected condition which prevented it from fulfilling the request.

### - What is a status code 202?

#### If the update is done asynchronous, this code can be used. It should include an URL to access the updated resource or an URL to check if the update has been succeeded

### - What is a status code 308?

#### This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future.

### - What code would you use if an update didn’t return data to a client?

#### 204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

### - What code would you use if a resource used to exist but no longer does?

#### 410 gone

### - What is the ‘Forbidden’ status code?

#### The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.
