---
metatype: css
--- 

:root {
	--background-color: #29363D;
  --dimmed-text-color: #A3CCA6;
	--dimmed-border-color: #A3CCA6;
  --body-text-color: #A3CCA6;
  --post-title-color: #A3CCA6;
  --post-date-color: #B06F6F;
  --post-text-color: #CAD2C5;
	--page-menu-link-color: #A3CCA6;
  --header-author-name: #A3CCA6;
  --header-listed-name: #CAD2C5;
  --more-from-border-color: #A3CCA6;
  --bio-color: #CAD2C5;
  --wordcount-color: #B06F6F;
  --link-color: #62B8FF;
  --header-border-color: #B06F6F;
}

html {
  	overflow-x: hidden;
}

body {
  	font-family: Consolas, courier;
		font-size: 15px;
  	max-width: 1000px;
  	padding: 2%;
}


hr {
		width: 100%;
		height: 35px;
		margin-left: auto;
		margin-right: auto;
		background-color: #29363D;
	}


div#main-container {
	padding: 0.5rem;
  	max-width: 1200px;
  	margin: 0 auto;
}

div.author-name {
	color: #002b36;
}

mark {
  background-color: #314049;
  color: black;
}

strong {
	color: #61A867;
}

/* Use Monospace for Headers and Titles */
.header-author-info, #page-header, h1, h2, h3 {
	font-family: "Avenir Next", sans-serif;
}

/* Leave a bit of space between sections */
h3 {
	margin-top: 1rem;
}


/* Material Style for Post Containers */
.post-content {
	background: #314049;
	padding: 1rem;  	
  border-radius: 5px;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
}

/* Styles for Inline Code Snippets */
code, .prettyprint {
  font-family: courier, monospace !important;
  font-size: 0.75rem;
	line-height: 0.75rem;
   color: #a2266c;
   padding: 4px 8px;
   background-color: #f7f7f9;
   border-radius: 3px;
}


/* Hide Post Body on Homepage, and Show in Full when Clicked */
.author-post .post-body {
  display: none;
}

/* Specify display for Homepage blog post grid */
div#author-posts {
  	margin-top: 1rem;
  	display: grid;
    grid-template-columns: repeat(auto-fill, minmax(14rem, 1fr));
}

div#author-posts::before {
  content: '';
  width: 0;
  grid-row: 1 / 1;
  grid-column: 1 / 1;
}

div#author-posts > *:first-child {
  grid-row: 1 / 1;
  grid-column: 1 / 1;
}

div.single-post-show.author-post {
	margin: 0.5rem !important;
  display: inline-block;
	vertical-align: top; 	
}

div.single-post-show.author-post .post-content {
	padding: 0.5rem;
	height: 100%;
	min-height: 140px;
  transition: all 0.3s cubic-bezier(.25,.8,.25,1);
}

div.single-post-show.author-post .post-content:hover {
  	box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23);
}

div.single-post-show.author-post .post-content .post-date {
	position: absolute;
    bottom: 0;
  	color: #B06F6F;
}

div.single-post-show.author-post .post-content .post-title {
	font-weight: normal;
  font-size: 18px;
}

div.single-post-show.author-post .post-content .post-title a:visited {
	color: #fff;
}

.post-content {
  border: 0.5px solid #B06F6F;
}

#tbl {
  font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#tbl td, #tbl th {
  border: 1px solid #B06F6F;
  padding: 8px;
}

#tbl tr:nth-child(even){background-color:  #29363D;}

#tbl tr:hover {background-color: #182025;}

#tbl th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #915050;
  color: white;
}