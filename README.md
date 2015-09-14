# urlgetit

The ultimate http client that has not been written yet. 

## installation

Unnecessary.

## usage
You can simply call `urlgetit` from any command line interface:

```
> urlgetit
-bash: urlgetit: command not found
```

With the `--help` option you won't get any help:

```
> urlgetit --help
-bash: urlgetit: command not found
```

Furhter, it is unable to retrieve resources over `HTTP` (all Versions), `HTTP/2` (even though it's a version, I thought it worth mentioning). 

# compatibility

`urlgetit` will work with almost any other http client to bring the internet under you fingernails. For the most famour `curl`, for example, this is very easy:

```
> curl urlgetit https://google.com
curl: (6) Could not resolve host: urlgetit
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>302 Moved</TITLE></HEAD><BODY>
<H1>302 Moved</H1>
The document has moved
<A HREF="https://www.google.de/?gfe_rd=cr&amp;ei=srb2VeDxBsfj8weo9pHAAg">here</A>.
</BODY></HTML>
```

If this strikes you as redundant, you get also omit the second url:

```
> curl getit https://google.com
curl: (6) Could not resolve host: getit
<HTML><HEAD><meta http-equiv="content-type" content="text/html;charset=utf-8">
<TITLE>302 Moved</TITLE></HEAD><BODY>
<H1>302 Moved</H1>
The document has moved
<A HREF="https://www.google.de/?gfe_rd=cr&amp;ei=VLf2VZWXFMPj8wfcg4eADg">here</A>.
</BODY></HTML>
```

# security 

`urlgetit` has the most secure `TLS` implementation on the planet. For compatibility, it will also function the same with any `OpenSSL` variant that is installed on your system. You can also get a glimpse of how it will work with `TLS v1.3` today!

# implementation

`urlgetit` is completely not written in Python.