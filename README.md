## Monocle

Monocle is a link and news aggregation website.

http://monocle.io

![Screenshot](http://maccman.github.io/monocle/screenshot.png)

### Prerequisites

* Ruby 2.0
* Postgres 9.3
* Redis
* A GitHub app account
* A Twitter app account

### Setup

    bundle install
    createdb monocle_development
    rake db:migrate

    export GITHUB_KEY=123
    export GITHUB_SECRET=123

    export TWITTER_KEY=123
    export TWITTER_SECRET=123
    
    thin start
    
    
###External Postgres

	export DATABASE_URL=postgres://external.db.host.com:5432/db

###External Memcached
    
	export MEMCACHE_URL=external.memcache.host.com:11211
	export MEMCACHE_USERNAME=user
	export MEMCACHE_PASSWORD=pass

###External Redis

	export REDIS_HOST=external.host.com
	export REDIS_PORT=6379
	export REDIS_PASSWORD=pass
	
