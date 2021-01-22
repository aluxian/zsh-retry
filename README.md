# retry

Retry a command up to a specific numer of times until it exits successfully, with exponential back off.

## Examples

```sh
$ retry 5 echo Hello
Hello
```

```sh
$ retry 5 false
Retry 1/5 exited 1, retrying in 1 seconds...
Retry 2/5 exited 1, retrying in 2 seconds...
Retry 3/5 exited 1, retrying in 4 seconds...
Retry 4/5 exited 1, retrying in 8 seconds...
Retry 5/5 exited 1, no more retries left.
```

## Credits

https://gist.github.com/sj26/88e1c6584397bb7c13bd11108a579746
