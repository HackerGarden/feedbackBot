feedbackBot 
========

The simplest feedback tool out there.
Include feedbackBot and receive screenshots, description and browser info straight in your github issues.

Built as a clone to Google's Feedback process

## Usage

Load jQuery, the plugin, and its CSS:
```html
    <script src="http://code.jquery.com/jquery-latest.min.js"></script>
    <script src="src/base64.js"></script>
    <script src="src/feedback.js"></script>
    <link rel="stylesheet" href="src/feedback.css" />
```

Init plugin:
```html
    <script type="text/javascript">
        $.feedback({
		html2canvasURL: 'src/html2canvas.js',
        	githubpath: 'ToolsforSociety/feedbackBot',
        	serverURL: 'http://feedbackbot.herokuapp.com'
      });
    </script>
```

## Requirements

* jQuery
* html2canvas
    
## Compatibility

Pretty much it should be working on any browser with `canvas` support. Browsers with no canvas support won't display the feedback button.

## License

feedbackBot is released under the MIT license. (See `LICENSE`)
