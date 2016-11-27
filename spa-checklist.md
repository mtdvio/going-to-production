# Single Page App Checklist

This is a checklist for browser-based Web App **without the backend** or with a 3rd-party backend.

## Legal

 - [ ] Licences of my app's 3rd-party dependencies are not violated
 - [ ] My app does not violate cryptography policies and laws  
 - [ ] My app is compliant according to the organisation standards

## Accessibility
 
 - [ ] My app is accessible
    - [ ] Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode
    - [ ] My app is screenreader-friendly
    - [ ] My app has keyboard navigation

## Deployment

 - [ ] My app is served from CDN or cookie-less subdomain
 - [ ] My app is server with forever cache headers for static assets
 - [ ] My app static resources are gzipped

## Loading optimization

 - [ ] My app can load it's assets in parallel (css, images and scripts)
 - [ ] My app uses icon sprites
 - [ ] My app does not hit [browser HTTP requests limit per host](http://stackoverflow.com/questions/985431/max-parallel-http-connections-in-a-browser)
 - [ ] My app loads all well-known javascript libraries from CDN

## Versioning

 - [ ] My app has a assets cache-busting implemented

## Assets

 - [ ] Have a 404-page
 - [ ] Have a maintenance page
 - [ ] Images support HDPI screens (Retina, etc)


## Testing

 - [ ] My app does not have memory leaks
 - [ ] My app is passing performance tests with high grades
    - [ ] [PageSpeed](https://developers.google.com/speed/pagespeed/) 
    - [ ] [YSlow](http://yslow.org/)
    - [ ] Chrome Dev Tools Audit

## Debugging

 - [ ] Minified JavaScript files contain URL for source maps
 - [ ] Thrown exceptions are handled and passed to storage ([Sentry](https://sentry.io/), [Track.js](https://trackjs.com/), etc)
 - [ ] Error storage process sourcemaped files

## Tracking

 - [ ] My app gathers metrics about usage behaviour

## Security
 - [ ] I have audited my system against:
    - [ ] OWASP Top 10 Vulnerabilities
    - [ ] [Observatory](https://observatory.mozilla.org/)
