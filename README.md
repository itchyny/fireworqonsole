Fireworqonsole
==============

A console to manage [Fireworq][] daemons on a Web UI.

> ![Screenshot](https://github.com/fireworq/fireworqonsole/raw/master/doc/images/console.png)

## <a name="start">Getting Started</a>

We are preparing to provide a pre-built binary.  For now, use a binary
generated by the following commands:

```
$ git clone https://github.com/fireworq/fireworqonsole
$ cd fireworqonsole
$ script/docker/build
```

You will get `./fireworqonsole`.  Make sure you have [Docker][] installed before running these commands.

If you want a binary other than for `linux-amd64`, you can specify `GOOS` and `GOARCH` environment variables.

```
$ GOOS=darwin GOARCH=amd64 script/docker/build
```

Run `fireworqonsole` by the following command.

```
$ ./fireworqonsole
```

Then access to http://localhost:8888/ from your browser and follow the instruction to add Fireworq nodes to manage.  You can also use `--node` argument of the command to specify nodes if you prefer.  To start a console with a different port, specify `--bind` argument of the command.

## <a name="license">License</a>

- Copyright (c) 2017 The [Fireworqonsole Authors][authors]. All rights reserved.
- Fireworq is licensed under the Apache License, Version 2.0. See
  [LICENSE][license] for the full license text.

[license]: ./LICENSE
[authors]: ./AUTHORS.md

[Fireworq]: https://github.com/fireworq/fireworq
[Docker]: https://www.docker.com/
