# Trackr

Trackr is a service to monitor the status and health of existing open and public trackers that anyone can use. A meta-tracker if you will. You can add any of the tracker announce URLs listed here to any of your torrents, or submit any other open/public trackers you might know of. 

# API

```
Get stable trackers:
Returns a two line delimited list of trackers that have an uptime of equal or more than 95%.

curl -X GET "https://trackr.0xc0d3.xyz/api/stable" -H "Accept: text/plain" 
```


```
Get working trackers:
Returns a two line delimited list of currently active and responding trackers.

curl -X GET "https://trackr.0xc0d3.xyz/api/live" -H "Accept: text/plain" 
```

```
Get trackers with given uptime:
Returns a two line delimited list of trackers that have an uptime of equal or more than the given percentage.

curl -X GET "https://trackr.0xc0d3.xyz/api/95" -H "Accept: text/plain" 
```

```
Get stable UDP trackers:
Returns a two line delimited list of stable UDP trackers.

curl -X GET "https://trackr.0xc0d3.xyz/api/udp" -H "Accept: text/plain" 
```

```
Get stable HTTP/HTTPS trackers:
Returns a two line delimited list of stable and HTTP/HTTPS trackers.

curl -X GET "https://trackr.0xc0d3.xyz/api/http" -H "Accept: text/plain" 
```

```
Get all trackers:
Returns a two line delimited list of all monitored trackers, dead or alive.

curl -X GET "https://trackr.0xc0d3.xyz/api/all" -H "Accept: text/plain" 
```
