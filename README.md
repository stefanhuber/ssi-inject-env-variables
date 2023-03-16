# Injecting Environment Variables with Docker into Static Webpages

In this example it is demonstrated how to inject environment variables into a static website. A more detailed description is found in [this blog post](https://www.stefanhuber.at/posts/ssi-inject-env-variables).

## Docker Build

```
docker build -t ssi-example .
```

## Docker Run

```
docker run --rm -it -p 9000:80 -e MY_NAME="world" -e MY_GREETING="hello" ssi-example
```