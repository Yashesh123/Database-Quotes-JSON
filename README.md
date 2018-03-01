# Database Quotes JSON

## JSON file with more than 1500+ famous quotes

### Below there are some examples, using jQuery and ES6, on how to work with this file

```javascript
// returns an array of all quotes with 12 words maximum
var filePath = "quotes.json";
$.getJSON(filePath)
	.done(
		data => data.filter(
			object => object.quoteText.split(" ").length <= 12
		)
	)

// returns an array of all quotes by Buddha
var filePath = "quotes.json";
$.getJSON(filePath)
	.done(
		data => data.filter(
			object => object.quoteAuthor === "Buddha"
		)
	)
```

## Donation
I'm hopeful this repo can help you! If so, please consider to offer me a coffee :)

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=L8CWHQLA5A9K8)
