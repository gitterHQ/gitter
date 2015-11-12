(Note to readers: some of our users have requested a changelog. This is experimental attempt at maintaining one)

## Redis Sentinel for Caching
### 13.10.2 (hotfix)

12 November 2015 16:46GMT

Our Redis caching instance has been moved to Redis Sentinel following an EC2 outage on our Redis caching master earlier today. Although our application caching infrastructure is designed to handle Redis outages, this was a sustained outage and eventually is caused the application to fail.

We have spun up some new Redis instances specifically for caching and switched caching to use Sentinel.

-- @suprememoocow
