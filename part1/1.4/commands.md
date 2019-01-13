# Commands

## Building Dockerfile

Execute:
```bash
$ docker build -t curler .
```

## Run the image

```bash
$ docker run -it --name=curler curler
```

Type `helsinki.fi` in your terminal and press enter. This produces output:

```text
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```