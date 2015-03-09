Webhook Demo Server
===================

Server built in tornado to demo the webhooks from a 3rd party.

Test locally:

* Open a browser to http://127.0.0.1:8888

To simulate an accepted response:
* curl -X POST -H "Content-Type: application/json" -d '{"object_id":"0","ts":"..."}' http://localhost:8888/a/callback/ok

To get an echo response:
* curl -X POST -H "Content-Type: application/json" -d '{"object_id":"0","ts":"..."}' http://localhost:8888/a/callback/echo

To simulate a 10 second timeout:

* curl -X POST -H "Content-Type: application/json" -d '{"object_id":"0","ts":"..."}' http://localhost:8888/a/callback/timeout

To simulate an error:

* curl -X POST -H "Content-Type: application/json" -d '{"object_id":"0","ts":"..."}' http://localhost:8888/a/callback/error

