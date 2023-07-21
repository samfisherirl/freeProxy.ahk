# freeProxy.ahk

- inspired by https://pypi.org/project/free-proxy/

- free working proxy from https://www.sslproxies.org/

- credit to thqby for winhttprequest https://github.com/thqby/ahk2_lib/blob/master/WinHttpRequest.ahk

```autohotkey

 example 1:
     proxyProp := freeProxy.retreive("US")
     ; united states can be passed but takes more time
     msgStr := proxyProp.IP ":" proxyProp.Port "`nHttps status: "
     msgStr .= ProxyProp.https ? "true" : "false"
     Msgbox(msgStr)

 example 2:
     proxyArrayofProps := freeProxy.retreive("US", arrayMode := 1) 
     ; ArrayMode provides entire list of proxies for the user to manipulate

     Msgbox(proxyArrayofProps[2].IP ":" ProxyArrayofProps[2].Port)

```
# notes

- Provide abbreviated country code for faster return
- Currently, a random number is used to return a Proxy from an array of proxies. 
 

# todo 

- add other sites: https://www.us-proxy.org/, https://free-proxy-list.net/uk-proxy.html and https://free-proxy-list.net 
- add elite/anon status
- https status
- concatenate string
