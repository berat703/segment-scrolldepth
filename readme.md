# Segment Scroll Depth
Segment Scroll Depth is a script that tracks how far users are scrolling on a page, and sends track events to [Segment](https://www.segment.com). The events can be sent to any Segment integration, including Google Analytics.

Segment Scroll Depth is a fork of [Scroll Depth](https://github.com/robflaherty/jquery-scrolldepth).

## Getting Started

1. Make sure Segment is installed on your site and that the Google Analytics integratoin is enabled.

2. Add `segment-scroll-depth.js` or `segment-scroll-depth.min.js` to your scripts folder.

3. Add the following code to any page where you want to track scroll depths as events in Segment.

```

<script src="path-to-script/segment-scroll-depth.min.js"></script>
<script>
jQuery(function() {
  jQuery.scrollDepth();
});
</script>

```

(Where `path-to-script` is the location of the script.)

That's it!

This script will send a tracking event to Segment when users scroll to 25%, 50%, 75%, and 100% of a page's length.

The `integrations` property tells Segment where to send these events. By default it is set to send only to Google Analytics, but you can change this to your preference.

## Contributing
Bug reports and code contributions are welcome. Please see [contributing.md](https://github.com/robflaherty/jquery-scrolldepth/blob/master/contributing.md).

## Contact
Twitter: [@grigoriy_kogan](https://twitter.com/grigoriy_kogan)
Web: [GKogan.co](http://www.gkogan.co)

## License
Licensed under the MIT and GPL licenses.