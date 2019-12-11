## Intro to PRAW

To use reddit api, you'll see configuration of the PRAW library at the top.

It uses 2 variables defined in `config.py` called `client_id` and `client_secret`.

The variables are left empty as good practice when version controlling.

You can get/find these value by going to: https://www.reddit.com/prefs/apps and signing into your reddit account that has a registered app. The next section will talk about acquiring the client id and secret.

Another parameter that PRAW takes to initialize is `user_agent`. It is recommended to always use a unique name, as this user_agent name is whats used to throttle/keep track of how many requests you make (which is 30 requests per minute).

## Getting a client id and secret

If you don't already have a client id and client secret, go to the above link and then follow these steps: https://github.com/reddit-archive/reddit/wiki/OAuth2.

Make sure that you register your app as a web app, if you wish to use it with PRAW.

After you have registered, you will have an app id and app secret (samething as client id and client secret).

Fill in those values in config.py, and the notebooks should be ready to run.


## More resources:
* https://www.reddit.com/dev/api/
* https://github.com/reddit-archive/reddit/wiki/API
* https://github.com/reddit-archive/reddit/wiki/OAuth2
* https://praw.readthedocs.io/en/latest/