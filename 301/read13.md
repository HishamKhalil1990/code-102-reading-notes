# SENDING FORM DATA
### when a client submit a form to server, it sends a request to the server using HTTP protocol. the server answer back by sending a response. forms define the sending method and where to send.
### 1. using the `action` attribute and putting the route `URL` , the data path is defined.
### 2. using the `method` attribute and putting one of `get` and `post` the sending process is defined.
### when using the `get` method, the data sent appended to the URL with an empty body, while when using `post` method the data are in the body and nothing appended to the URL. in both cases the data is sent as pairs key/value.
### forms are constructed of inputs field `<input>` and buttons `<button>`
