# What is Erlang?

Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability. Some of its uses are in telecoms, banking, e-commerce, computer telephony and instant messaging. Erlang's runtime system has built-in support for concurrency, distribution and fault tolerance.

> [wikipedia.org/wiki/Erlang_(programming_language)](https://en.wikipedia.org/wiki/Erlang_%28programming_language%29)

%%LOGO%%

# How to use this image

## Create a `Dockerfile` in your Erlang app project

```dockerfile
FROM erlang:18-onbuild
```

Then, build and run the Docker image:

```console
$ docker build -t my-erlang-app .
$ docker run -it --rm --name my-running-app my-erlang-app
```

## Run a single Erlang escript

```console
$ docker run -it --rm --name %%REPO%%-inst1 -v "$PWD":/usr/src/myapp -w /usr/src/myapp %%REPO%% escript your-escript.erl
```
