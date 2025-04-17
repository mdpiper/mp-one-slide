# one-slide-bio

A one-slide bio.

Present this slide with [reveal-md](https://github.com/webpro/reveal-md) through their public Docker image:
```
git clone https://github.com/mdpiper/one-slide-bio
docker run --rm -p 1948:1948 -p 35729:35729 -v $PWD/one-slide-bio:/slides webpronl/reveal-md:latest /slides --watch
```
The service is now running at http://localhost:1948.

To build a static website for this slide,
[install reveal-md](https://github.com/webpro/reveal-md#installation) and run:
```
reveal-md slide.md --static _site
```
Then move `_site` to the webroot directory.
