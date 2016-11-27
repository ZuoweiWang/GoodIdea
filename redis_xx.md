### Install with Homebrew

    brew install redis

Set up launchctl to auto start `redis`

    $ ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents

`/usr/local/opt/redis/` is a symlink to `/usr/local/Cellar/redis/x.y.z` (e.g., `2.8.7`)

You can use launchctl to start and stop `redis`

    $ launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist
    $ launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.redis.plist
    
You can also more conveniently use `brew` to start, stop, and verify service status

    $ brew services list | grep redis
    $ brew services start redis
    $ brew services stop redis

#### Notes

The default plist provided by homebrew stores the redis configuration at `/usr/local/etc/redis.conf`.

For more about `launchctl` see:

https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/launchctl.1.html#//apple_ref/doc/man/1/launchctl

http://launchd.info/




➜ ✗ ps aux | grep "redis-server"

--
jasdeep        98081   0.0  0.0  2564132    100   ??  S    Wed10am   6:56.33 redis-server

--
➜  ✗ kill -9 98081

--
[Mac下配置redis](https://davidwangtm.github.io/2016/07/20/mac_redis_introduction/)


 
