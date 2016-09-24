# Single Page App Checklist

This is a checklist for browser-based Web App **without the backend** or with a 3rd-party backend.

## Legal

 - [ ] Licences of my app's 3rd-party dependencies are not violated
 - [ ] My app does not violate cryptography policies and laws  
 - [ ] My app is compliant according to the organisation standards

## Accessibility
 
  - [ ] My app is accessible

    - Colors and contrast are color-blind friendly OR there is a possiblity to switch to high-contrast mode
    - My app is screenreader-friendly
    - My app has keyboard navigation

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

 - [ ] My app has a cache-busting implemented 


## Testing

 - [ ] My app is passing performance tests with high grades
   - [PageSpeed](https://developers.google.com/speed/pagespeed/) 
   - [YSlow](http://yslow.org/)
   - Chrome Dev Tools Audit

 - [ ] My app does not have memory leaks

## Debugging

 - [ ] minified JavaScript files contain URL for source maps

## Tracking

 - [ ] My app gathers metrics about usage behaviour
