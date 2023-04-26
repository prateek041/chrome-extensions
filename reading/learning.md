# What I have learnt while building this

- The images are needed for different sizes like webstore and browsers for different OS.

## Content Scripts

Content scripts run in an isolated world, i.e. they cannot be accessed by outside world and the other extensions.

## Match pattern

It is about selecting what urls we want our extension to run for. so, we define a pattern in the form of

```regex
<url-patter> := <scheme>:<host><path>
<scheme> := '*' | 'http' | 'https' | 'file' | 'ftp' | 'urn'
<host> := '*' | '*.' <any char except '/' and '*'>+
<path> := '/' <any chars>
```
