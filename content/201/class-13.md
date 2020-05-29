# Local Storage

---

**HTML5 storage**, or **web storage**, is a way to store key-value pairs locally in the browser.

`setItem()` and `getItem()` can be used to give and take from the local storage.

---

#### Limitations

- 5 megabytes by default across browsers
- `QUOTA_EXCEED_ERR` is thrown when over 5 megabytes is used
- There can not be a request for more storage

---

#### More Storage Information

Using this local storage, a browser can be exited without any inputted information being lost. If a game is running off of local storage, the browser can be exited and re-entered within the same spot in the game.

Unlike cookies, information stored locally is not sent back to the web server.