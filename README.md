GitHub Mood Light
============

Mood Light and Music triggered by github events

Check it out at [https://github-mood-light.herokuapp.com](https://github-mood-light.herokuapp.com)

Dependencies
---------------------
* node
* npm
* redis

Environment variables
---------------------

```
$ export GITHUB_OAUTH_KEY=<your_github_oauth_key>
```
Note: Without the GitHub oauth key the number of requests is throttled at 60 per hour. It can be increased to 5000 per hour by using an oauth key.

Run Redis and Server
----------

```bash
$ redis-server
```

In a separate window:

```bash
$ node server
```

Note: For production run `export NODE_ENV="production"` before starting the server.


#### Todo
- [x] Add Mood Light
- [ ] Dockerize
- [x] Deploy
- [ ] Clean up / Modularize code

---------------------
This is extended from [Github Audio Project](https://github.com/debugger22/github-audio)<br>
Check it out at [https://github.audio/](https://github.audio/)