xhyvedocker
===========

WARNING THIS IS AN EVIL HACK. I might not overwrite anything of yours that's important if you run this. _might_.

`xhyvedocker` is a script with similar purpose to `boot2docker`'s CLI, only running boot2docker under xhyve instead of virtualbox.  All the caveats of xhyve apply.

I assume you're using homebrew. Plan accordingly.

Use
----

Install the dependencies with homebrew:

```bash
xyvedocker deps
```

Initialize and start.


```bash
xhyvedocker init
xhyvedocker start
```

Then wait for boot.

Pay attention to the network address readout. Press `Control-\` to detach the console when you're done.

next, extact the keys:

```bash
xhyvedocker keys
```

And then run docker.

```bash
docker -H 192.168.64.x:2376 --tls=true info
```
