<h1>Why AFS.one?</h1>
<p>
We wanted to create a collaborative repository highlighting success cases of
Enterprise Free Software Publishers with a focus on those companies that actually
create it and a bias towards <b>real Free software</b> - software that users 
can actually modify, fix, improve or share.
</p>

<p>
Target Audience are Enterprises willing to implement Free Software with all the
warranties and long term commitment provided by a Commercial Software Publisher.
</p>

<p>
The idea of <a href="http://www.afs.one/" title="AFS | Awesome Free Software">AFS</a>
was not create yet another directory of Open Source/Free Software such as
<a href="http://freecode.com/">freecode</a> or another guide of supposed
Open Source Software, that uses the term &quot;Open Source&quot; as a marketing
argument to promote proprietory software that cannot be modified, fixed, improved
or shared.
</p>

<p>
Our ultimate goal is to ensure that Enterprises can take control of their IT
through Free Software and reduce their risks thanks to this model of publishing.
</p>

<h1>How to contribute?</h1>
<p>Submit pull requests following the JSON scheme described below.</p>


<h1>JSON Schema</h1>
<p>All JSON text entries must use UTF-8 encoding.</p>
<p>
Each publisher has a single JSON file with straightforward properties. Notables:
</p>

<ul>
  <li><code>country</code>: origin country of the publisher (<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">ISO 3166-1 alpha-2</a>)</li>
  <li><code>presence</code>: countries the publisher has a presense (<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">ISO 3166-1 alpha-2</a>)</li>
  <li><code>source_code_download</code>: link to an archive with all source code available under a Free Software license</li>
  <li>
    <code>commercial_support</code>: link to a resource/page describing the type of commerical support provided for the respective Free Software
    (empty if commercial support is only available for another (version of the) software that can be downloaded using <code>source_code_download</code>).  
  </li>
  <li>wikipedia_url: link to the wikipedia page of the Free Software</li>
  <li>openhub_url: link to the openhub page of the Free Software</li>
  <li>language: the language of a success case (<a href="https://en.wikipedia.org/wiki/ISO_639-1">ISO 639-1</a>)</li>
</ul>
<p>
The full JSON schema is here:
</p>
<pre><code>
{
	"title": [company title],
	"logo": [url to company logo],
	"country": [origin country of the publishe],
	"presence": [countries the publisher has a presense, e.g. ["us", "gb"]],
	"website": [url to company website],
	"founded_year": [year company was founded],
	"free_software_list": [{
		"title": [software title],
		"logo": [url to software logo],
		"category_list": [list of categories, e.g. ["communication", "database"]],
		"source_code_download": [link to an archive with all source code],
		"commercial_support": [link to a resource/page describing the type of commerical support provided],
		"wikipedia_url": [link to the wikipedia page of the Free Software],
		"success_case_list": [{
			"title": [title of success case],
			"image": [url to screenshot of success case],
			"customer": [name of client/customer],
			"country": [country of origin of customer],
			"language": [language of success case],
			"url": [url to success case]
		}, {
			[...next success case...]
		}]
	}, {
	  [... next Free Software ...]
	}]
}
</code></pre>


<h1>Software Categories</h1>
<p>
Free Software is categorized using the following terms:
</p>
<ul>
	<li>communication (email, chat, videoconferencing, etc.)</li>
	<li>database (SQL, NoSQL, etc.)</li>
	<li>application (ERP, CRM, e-commerce, project management, etc.)</li>
	<li>analytics (big data, machine learning, data visualisation, etc.)</li>
	<li>developer (text editor, IDE, frameworks)</li>
	<li>gis (map editor, map visualisation)</li>
	<li>desktop (desktop operating system, desktop web browser, desktop VM, etc.)</li>
	<li>mobile (mobile operating system, mobile web browser, mobile VM, etc.)</li>
	<li>middleware (ESP, ETL, ELT, etc.)</li>
	<li>infrastructure (public cloud, private cloud, software defined network, hyperconverged OS, IOT management)</li>
</ul>
<p>
Categories have been chosen on purpose taking into account the increaing convergence in IT:
</p>

<ul>
	<li>application convergence (ERP, CRM, Web, Project, Big Data)</li>
	<li>infrastructure convergence (server OS, networking, routing, hyperconverged OS)</li>
	<li>desktop convergence (desktop OS, web browser, VM)</li>
	<li>mobile convergence (mobile OS, mobile browser, VM)</li>
	<li>middleware (ESB, ETL, etc.)</li>
</ul>

<p>
The difference between application and communication, for example, is that 
application is persistent and communication is not. Email messaging can thus be 
considered in some cases as communication and in other cases as application
(such as in a CRM).
</p>

