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
        	githubpath: 'ToolsforSociety/feedbackBot', // CHANGE THIS TO YOUR PATH
	        serverURL: 'http://feedbackbot.herokuapp.com' // YOU CAN HOST YOUR OWN GITHUB BOT IF YOU WANT
      });
    </script>
```

Add the button
```html
 <button class="feedback-btn feedback-btn-blue">Feedback</button>
```

## Requirements

* jQuery
* html2canvas
    
## Compatibility

Pretty much it should be working on any browser with `canvas` support. Browsers with no canvas support won't display the feedback button.

## License

feedbackBot is released under the MIT license. (See `LICENSE`)
