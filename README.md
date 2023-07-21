# freeProxy.ahk

inspired by https://pypi.org/project/free-proxy/

credit to thqby for winhttprequest https://github.com/thqby/ahk2_lib/blob/master/WinHttpRequest.ahk

```autohotkey

; example

ProxyProp := freeProxy.retreive("US") ; full country list in class, full names can be passed but takes longer

Msgbox(ProxyProp.IP ":" ProxyProp.Port)

```
# notes

- Provide abbreviated country code for faster return
- Currently, a random number is used to return a Proxy from an array of proxies. 

inspired by https://pypi.org/project/free-proxy/
free working proxy from https://www.sslproxies.org/

# todo 

add other sites: https://www.us-proxy.org/, https://free-proxy-list.net/uk-proxy.html and https://free-proxy-list.net 
add elite/anon status
https status
concatenate string
