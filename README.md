## webshotter

A very simple Python script to take screenshots of websites. It can be
handy in internal security assessments where several hosts have HTTP
servers, so one can use it to narrow down their target to the interesting
applications and weed out less interesting ones as well as default HTTP
pages. Can also be useful for bug bounty hunters when scanning for
applications running in obscure subdomains.

## Usage

```
usage: webshotter.py [-h] [-x HEIGHT] [-y WIDTH] [-t THREADS] [-v] urllist
```

Sample usage - starts the tool with 3 threads and verbose mode:

```
julio@blaze:~/tools/web/webshotter$ ./webshotter.py -v urls.txt -t 3
Starting with 3 threads
Thread-3 received argument: http://www.whatever.io
Thread-2 received argument: http://www.google.com
Thread-1 received argument: http://www.blazeinfosec.com
Thread-1 received argument: http://www.twitter.com
Thread-1 received argument: http://www.facebook.com
Thread-1 received argument: http://www.reddit.com/r/netsec
Thread-1 received argument: http://blog.whatever.io
```

## Dependencies

This code depends on Selenium Web Driver and PhantomJS.

## Known issues

Nothing yet.

## Contributors

Send a pull request if you feel like.

## Author

* **Julio Cesar Fort** - julio at blazeinfosec dot com
* Twitter: @juliocesarfort / @blazeinfosec

## License

This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.

