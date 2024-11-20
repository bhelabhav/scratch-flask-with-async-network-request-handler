This is a simple test app to batch requests to an external api over HTTP
asynchronously while using a synchronous flask application.

The async requests are ultimately awaited within the scope of the sync
flask request.

Future behaviors I'd like to test (and maybe rename the repo someday) is
comparison of frameworks and different async architectures that are more
robust e.g.


Server -> pubsub -> message queue -> queue subscriber

Server -> pubsub -> topic subscriber

Server -> message queue -> queue subscriber


And using celery / no celery.

And comparing the different pros/cons and also making setup relatively easy
to do.

...

