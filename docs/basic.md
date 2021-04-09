
<!doctype html>
<!--[if lt IE 7]>
<html class="no-js lt-ie9 lt-ie8 lt-ie7" lang="en"> <![endif]-->
<!--[if IE 7]>
<html class="no-js lt-ie9 lt-ie8" lang="en"> <![endif]-->
<!--[if IE 8]>
<html class="no-js lt-ie9" lang="en"> <![endif]-->
<!--[if gt IE 8]><!-->
<html class="no-js" lang="en"> <!--<![endif]-->
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">

	<title>Numeral.js</title>
	<meta name="description"
		  content="A javascript library for formatting and manipulating numbers.">
	<meta name="author" content="">

	<link rel="shortcut icon" href="/favicon.ico" type="image/x-icon">
	<link rel="icon" href="/favicon.ico" type="image/x-icon">

	<meta name="viewport"
		  content="initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0">

	<link rel="stylesheet" href="css/build/style.css">

	<script type="text/javascript">

		var _gaq = _gaq || [];
		_gaq.push(['_setAccount', 'UA-35249784-1']);
		_gaq.push(['_setDomainName', 'numeraljs.com']);
		_gaq.push(['_setAllowLinker', true]);
		_gaq.push(['_trackPageview']);

		(function() {
			var ga = document.createElement('script');
			ga.type = 'text/javascript';
			ga.async = true;
			ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
			var s = document.getElementsByTagName('script')[0];
			s.parentNode.insertBefore(ga, s);
		})();

	</script>
</head>
<body class="cf">
<!--[if lt IE 7]><p class=chromeframe>Your browser is <em>ancient!</em> <a
		href="http://browsehappy.com/">Upgrade to a different browser</a> or <a
		href="http://www.google.com/chromeframe/?redirect=true">install Google
	Chrome Frame</a> to experience this site.</p><![endif]-->
<div class="header-bar full"></div>
<div class="sidebar thrd m-full s-full">
	<div class="inner">
		<h1 class="logo">
			Numeral.js
		</h1>

		<p class="tagline">
			A javascript library for formatting and manipulating numbers.
		</p>

		<p id="version">
		</p>

		<div id="nav" class="nav"></div>
		<div class="github-links">
			<a class="button flat"
			   href="https://github.com/adamwdraper/Numeral-js"><i
					aria-hidden="true" class="icon-github"></i> Github</a>
			<a class="button flat download"
			   href="https://github.com/adamwdraper/Numeral-js/zipball/master"><i
					aria-hidden="true" class="icon-download"></i> .ZIP</a>
			<a class="button flat download"
			   href="https://github.com/adamwdraper/Numeral-js/tarball/master"><i
					aria-hidden="true" class="icon-download"></i> .TGZ</a>
		</div>
		<label for="language-select">Language</label>
		<select id="language-select" name="language-select">
			<option value="chs">Chinese</option>
			<option value="cs">Czech</option>
			<option value="dk">Danish</option>
			<option value="be-nl">Dutch (Belgium)</option>
			<option value="en" selected="selected">English</option>
			<option value="en-gb">English (Great Britain)</option>
			<option value="fi">Finnish</option>
			<option value="fr">French</option>
			<option value="de-de">German</option>
			<option value="de-de">Italian</option>
			<option value="ja">Japanese</option>
			<option value="pt-pt">Portuguese (Portugal)</option>
			<option value="pt-br">Portuguese (Brazil)</option>
			<option value="ru">Russian</option>
			<option value="es">Spanish</option>
			<option value="th">Thai</option>
			<option value="tr">Turkish</option>
		</select>

		<div id="carbonads-container" class="ad-container">
			<div class="carbonad">
				<div id="azcarbon"></div>
				<script type="text/javascript">
					var z = document.createElement("script");
					z.type = "text/javascript";
					z.async = true;
					z.src = "http://engine.carbonads.com/z/51885/azcarbon_2_1_0_HORIZ";
					var s = document.getElementsByTagName("script")[0];
					s.parentNode.insertBefore(z, s);
				</script>
			</div>
		</div>
	</div>
</div>
<div class="content xl-over-thrd l-over-thrd thrd2 m-full s-full">
<div class="inner">

<h3>Use it</h3>
<h4>In the Browser</h4>
<pre>
&lt;script src=&quot;numeral.min.js&quot;&gt;&lt;/script&gt;
</pre>
or include from cdnjs.com
<pre>
&lt;script
    src=&quot;//cdnjs.cloudflare.com/ajax/libs/numeral.js/1.5.3/numeral.min.js&quot;&gt;&lt;/script&gt;
</pre>
<h4>In Node.js</h4>
<pre>
npm install numeral
</pre>
<pre>
var numeral = require('numeral');
</pre>

<h3>Format</h3>

<p>
	Numbers can be formatted to look like currency, percentages, times, or even
	plain old numbers with decimal places, thousands, and abbreviations.
</p>
<pre>
var string = numeral(1000).format('0,0');
// '1,000'
</pre>
<h4>Numbers</h4>
<table id="format-numbers" class="table striped bordered">
	<thead>
	<tr>
		<th>Number</th>
		<th>Format</th>
		<th>String</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h4>Currency</h4>
<table id="format-currency" class="table striped bordered">
	<thead>
	<tr>
		<th>Number</th>
		<th>Format</th>
		<th>String</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h4>Bytes</h4>
<table id="format-bytes" class="table striped bordered">
	<thead>
	<tr>
		<th>Number</th>
		<th>Format</th>
		<th>String</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h4>Percentages</h4>
<table id="format-percentage" class="table striped bordered">
	<thead>
	<tr>
		<th>Number</th>
		<th>Format</th>
		<th>String</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h4>Time</h4>
<table id="format-time" class="table striped bordered">
	<thead>
	<tr>
		<th>Number</th>
		<th>Format</th>
		<th>String</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h3>Unformat</h3>

<p>
	Got a formatted string? Use the unformat function to make it useful again.
</p>
<pre>
var string = numeral().unformat('($10,000.00)');
// -10000
</pre>
<table id="unformat-all" class="table striped bordered">
	<thead>
	<tr>
		<th>String</th>
		<th>Function</th>
		<th>Number</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h3>Manipulate</h3>

<p>
	Not that you will use these often, but they're there when you need them.
</p>
<pre>
var number = numeral(1000);

var added = number.add(10);
// 1010
</pre>
<table id="manipulate" class="table striped bordered">
	<thead>
	<tr>
		<th>Before</th>
		<th>Function</th>
		<th>After</th>
	</tr>
	</thead>
	<tbody></tbody>
</table>
<h3>Value</h3>

<p>
	The value is always available.
</p>
<pre>
var number = numeral(1000);

var string = number.format('0,0');
// '1,000'

var value = number.value();
// 1000
</pre>
<h3>Set</h3>

<p>
	Set the value of your numeral object.
</p>
<pre>
var number = numeral();

number.set(1000);

var value = number.value();
// 1000
</pre>
<h3>Difference</h3>

<p>
	Find the difference between your numeral object and a value
</p>
<pre>
var number = numeral(1000),
    value = 100;

var difference = number.difference(value);
// 900
</pre>
<h3>Default Formatting</h3>

<p>
	Set a default format so you can use .format() without a string. The default
	format to '0,0'.
	<br>This value can be set when defining a language.
</p>
<pre>
var number = numeral(1000);

number.format();
// '1,000'

numeral.defaultFormat('$0,0.00');

number.format();
// '$1,000.00'
</pre>
<h3>Currency Default Formatting</h3>

<p>
	Set a default currency format so you can use .formatCurrency() without a
	string. The default format to '0.00'.
	<br>This value can be set when defining a language.
</p>
<pre>
var number = numeral(1000);

number.formatCurrency();
// '1,000.00'

numeral.defaultFormat('$0,0.00');

number.formatCurrency();
// '$1,000.00'
</pre>
<h3>Custom Zero Formatting</h3>

<p>
	Set a custom output when formatting numerals with a value of 0
</p>
<pre>
var number = numeral(0);

numeral.zeroFormat('N/A');

var zero = number.format('0.0')
// 'N/A'
</pre>
<h3>Clone</h3>

<p>
	Go ahead and clone any numeral object while you're at it.
</p>
<pre>
var a = numeral(1000);
var b = numeral(a);
var c = a.clone();

var aVal = a.set(2000).value();
// 2000

var bVal = b.value();
// 1000

var cVal = c.add(10).value();
// 1010
</pre>
<h3>Languages</h3>

<p>
	Lets make this useable all over the place!
</p>
<pre>
// load a language
numeral.language('fr', {
    delimiters: {
        thousands: ' ',
        decimal: ','
    },
    abbreviations: {
        thousand: 'k',
        million: 'm',
        billion: 'b',
        trillion: 't'
    },
    ordinal : function (number) {
        return number === 1 ? 'er' : 'ème';
    },
    currency: {
        symbol: '€',
        position: 'postfix' // 'prefix'/'infix'/'postfix'. Default is 'prefix'
        spaceSeparated: 'true' // 'true'/'false'. Default is 'false'
    },
    defaults: {
        format: '0.00',
        currencyFormat: '0[.]00a'
    }
});

// switch between languages
numeral.language('fr');
</pre>
<p>
	As I am not fluent in every language on the planet, please feel free to
	create language files of your own by submitting a pull request. Don't forget
	to create both the language file (example: languages/fr.js) and the language
	test (example: tests/languages/fr.js). Thanks for helping out.
</p>

<h3>Acknowlegements</h3>

<p>
	Numeral.js, while less complex, was inspired by and heavily borrowed from <a
		href="http://momentjs.com/">Moment.js</a>
</p>

</div>
</div>

<div class="footer l-thrd xl-thrd full">
	<div class="inner">
		<p>
			This is a project by <a href ="https://github.com/adamwdraper/Numeral-js">Företagsplatsen</a> forked from
			<a href="http://github.com/adamwdraper">adamwdraper</a>/<a href="https://github.com/adamwdraper/Numeral-js">Numeral-js</a>

		</p>
	</div>
</div>
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.8.1/jquery.min.js"></script>
<script src="./js/min/site.min.js"></script>
</body>
</html>