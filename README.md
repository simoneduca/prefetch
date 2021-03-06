# prefetch

Illustrate basic service workers usage (registration and actica) to serve cached content.

More details:

If the browser supports service workers, a Service Worker is registered and activated.
The SW then prefetch one resource and store it in the cache using the [Cache API](https://developer.mozilla.org/en-US/docs/Web/API/Cache).
When offline, the SW will serve the the prefetched resource from the cache.

Important: Service Workers are scripts running in the browser and hence a potential security hazard.
For that reason they must be served over HTTPS.

To try this out:

(Only available locally for now, because Github Pages are not served over HTTPS. [See the error for yourself](http://www.simoneduca.com/prefetch)):

1. Clone the repo and run it locally

2. Click on the prefetch links while online. Happy days.

3. Go offline.

4. Click on the links again: the first will serve the cached image but the second will not.

5. Party.

Disclaimer: I lifted most of the code from [here](https://github.com/GoogleChrome/samples/tree/gh-pages/service-worker/prefetch).

[![Feature Requests](http://feathub.com/simoneduca/prefetch?format=svg)](http://feathub.com/simoneduca/prefetch)
