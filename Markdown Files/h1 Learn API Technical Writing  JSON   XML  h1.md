<h1>Learn API Technical Writing: JSON & XML</h1>
<p>JavaScript Object Notation (JSON) features several basic data types:</p>
<ul>
	<li>Strings - Enclosed in single or double quotation marks (“ “)</li>
	<li>Number - Integer or decimal, positive or negative</li>
	<li>Booleans - True/False statements without quotation marks</li>
	<li>Null - Meaning nothing, without quotation marks</li>
</ul>
<p>In addition to the basic data types, JSON also features Arrays and Objects<p>
<h2>Arrays:</h2>
<ul>
	<li>Arrays are lists and feature the [ ] notation</li>
	<li>Elements within an Array are separated by commas</li>
	<li>Able to mix data types - EX: [12, -3, 17, null]</li>
</ul>
<h2>Objects:</h2>
<ul>
	<li>Objects are JSON’s dictionaries and are enclosed in { } notation</li>
	<li>Keys/Values are separated by ( : ), pairs are separated by commas</li>
	<li>Able to be any data type - EX: {“red”:205, “green”:117, “blue”: 53}
<h2>Nesting:</h2>
<p>Involves putting arrays and objects inside each other</p>
<ul>
	<li>Arrays can be placed inside objects, objects inside arrays, arrays inside of arrays, etc</li>
	<li>Often, a JSON file is one big object with lots of objects and arrays inside</li>
	<li>Ex: JSON Description of a Song</li>
	

{
“Song”
	{
		“title”: “Hey Jude”,
		“srtist”: ”The Beatles”,
“musicians”: 
[“John Lennon”, “Paul McCartney”, “George Harrison”, “Ringo Starr”]
            }
} 



<p>eXtensible Markup Language (XML)</p>
<ul>
	<li>Similar to HTML - used for creating websites</li>
	<li>XML can be used for any kind of structured data</li>
</ul>
<h2>Tags</h2>
<ul>
	<li>Start tags format - EX: < __ ></li>
	<li>End tags format - EX: </ __ ></li>
	<li>Tag names must only be letters, numbers, and underscores</li>
</ul>
<h2>Content</h2>
<ul>
	<li>Information that goes between the tags is considered content</li>
	<li>Content without tags is considered a string - even without quotes</li>
	<li>If content has tags - Nest the data: tags inside of tags to create nested data</li>
</ul>
``` 
<color>
<red>504</red>
	<green>123</green>
	<blue>42</blue>
</color>
<h2>Attribute</h2>
<ul>
	<li>In addition to content, tags can have attributes</li>
	<li>Attributes are key/value pairs</li>
	<li>Both are strings, but key <strong>do not have quotes</strong> - only the values have quotes</li>
	<li>Keys must be letters, numbers, and underscores only</li>
	<li>No spaces of punctuation between characters</li>
	<li>Attributes appear in the start tag - key=”value”</li>
	<li>Most common designs <strong>do not</strong> feature attributes for data</li>
	<li>Used to indicate that some property about the data - metadata</li>
```
<fileSize unit=”KB”>34.6</fileSize>
<cost currency=”USD”>42.3</cost>
<projectedValue decimals=”2” confidence=”5”>23.5</projectedValue>
<h2>Namespaces</h2>
<p>Tags could mean one thing in one context, but something entirely different in a different context</p>
<ul>
	<li>For this, identify unique tags with namespaces</li>
	<li>Features a “namespace:” prefix</li>
		<li>EX: <”contentWithTheTechnical:” Notes></li>
</ul>
<h2>White space and Indentation</h2>
<p>”White space” means spaces, new lines, etc</p>
<p>Good XML Formatting</p>
<ul>
	<li>General: add indent for every new level of brackets</li>
	<li>Tags that <strong>do not</strong> contain other tags can have start/end tags on the same line</li>
	<li>Tags that contain other tags should be on their own line</li>
</ul>
<h2>Tools for Writing Structured Data Documentation</h2>
<p>Word processors, such as Microsoft Word, are simple to use and offer a clean, nice looking document</p>
<ul>
	<li>Lacks accessibility across the web</li>
	<li>Provides Track Changes and Comment functionality</li>
</ul>
<p>Types of Web-based content</p>
<ul>
	<li><strong>Markdown</strong></li>
	<li>API documentation can be crafted in HTML, but can be tedious and hard to read until put into a browser</li>
	<li><strong>Common Markup Language:</strong></li>
	<li><strong>Markdown</strong> - simpler than standard HTML and works well with most structured data documentation types</li>
	<li><strong>Wikis</strong></li>
	<li>Simple content system, easy for multiple writers to contribute to the same documentation</li>
	<li>Commonly used for internal documentation</li>
	<li>Example Tools: MediaWiki, TWiki, <strong>Confluence</strong>, and MindTech</li>
	<li><strong>Commercial Tools</strong></li>
	<li>Many commercial tools are available for API documentation</li>
	<li>Able to produce content in both HTML and PDF formats</li>
	<li>Example Commercial Tools: <strong>Flare</strong>, RoboHelp, and Help & Manual</li>
</ul>
