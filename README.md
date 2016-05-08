This is a fork of [aelvan's AutoMin plugin](https://github.com/aelvan/AutoMin-Craft) which adds cache-breaking functionality for when .scss @imports (includes) are modified.

---

Because the plugin loops through every .scss file that exists in your 'include path' directory and detects each file's last modified time, the cache-break check is restricted to only while Craft is in Dev Mode.

The @imports should all be in the same directory. Any modifications to @imported files will subsequently change the 'last modified time' on all .scss files in your templates that are passed to AutoMin.
