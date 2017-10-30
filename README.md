# SpringRestServiceExample
Spring Rest Service to count the number of words Example


To Setup application 
	use "mvn install" to build application
	use "web.xml" to deploy application
	use sampleParagraph.txt to load new text

URL 1
Post Request
http://localhost:8080/CountWordByRESTSpring/rest/search
Basic Authorization Header
Basic b3B0dXM6Y2FuZGlkYXRlcw==

Input
{
  "searchText": [
    "Duis",
    "Sed",
    "Donec",
    "Augue",
    "Pellentesque",
    "123"
  ]
}

Output
{
"wordCounts": {
123: 0,
"Sed": 0,
"Donec": 0,
"Augue": 0,
"Pellentesque": 0,
"Duis": 0
}
}

URL 2 To get top word counts
Get Request
http://localhost:8080/CountWordByRESTSpring/rest/top/{count}
Basic Authorization Header
Basic b3B0dXM6Y2FuZGlkYXRlcw==

Output will top {count} word count 
