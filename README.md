<h1>Why AFS.one?</h1>
<p>
We wanted to create a collaborative repository highlighting success cases of
Enterprise Free Software Publishers with a focus on those companies that actually
create it and a bias towards <b>real Free software</b> - software that users 
can actually modify, fix, improve or share.
</p>

<p>
Target Audience are Enterprises willing to implement <a href="https://www.gnu.org/philosophy/free-sw.en.html">Free Software</a> with all the
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
Each publisher has a single JSON file with straightforward properties. Notable properties::
</p>

<ul>
  <li><code>country</code>: origin country of the publisher (<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">ISO 3166-1 alpha-2</a>)</li>
  <li><code>presence</code>: countries the publisher has a presense (<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">ISO 3166-1 alpha-2</a>)</li>
  <li><code>source_code_download</code>: link to an archive with all source code available under a <a href="https://www.gnu.org/licenses/license-list.en.html">Free Software license</a></li>
  <li><code>source_code_profile</code>: link to the <a href="https://www.openhub.net/">openhub</a> source code profile</li>
  <li>
    <code>commercial_support</code>: link to a page describing the type of commerical support provided for the respective Free Software
    (empty if commercial support is only available for another (version of the) software than the one that can be downloaded using <code>source_code_download</code>).  
  </li>
  <li><code>wikipedia_url</code>: link to the <a href="https://www.wikipedia.org/">wikipedia</a> page of the Free Software</li>
  <li><code>language</code>: the language of a success case (<a href="https://en.wikipedia.org/wiki/ISO_639-1">ISO 639-1</a>)</li>
</ul>
<p>
The full JSON schema is here:
</p>
<pre><code>
{
        "title": &lt;&lt;company title&gt;&gt;,
        "logo": &lt;&lt;url to company logo&gt;&gt;,
        "country": &lt;&lt;origin country of the publishe&gt;&gt;,
        "presence": &lt;&lt;countries the publisher has a presense, e.g. ["us", "gb"]&gt;&gt;,
        "website": &lt;&lt;url to company website&gt;&gt;,
        "founded_year": &lt;&lt;year company was founded&gt;&gt;,
        "free_software_list": [{
                "title": &lt;&lt;software title&gt;&gt;,
                "logo": &lt;&lt;url to software logo&gt;&gt;,
                "website": &lt;&lt;software website&gt;&gt;,
                "category_list": &lt;&lt;list of categories, e.g. ["Developer", "Communication"]&gt;&gt;,
                "source_code_download": &lt;&lt;link to an archive with all source code&gt;&gt;,
                "source_code_profile": &lt;&lt;link to openhub source code profile&gt;&gt;,
                "commercial_support": &lt;&lt;link to a resource/page describing the type of commerical support provided&gt;&gt;,
                "wikipedia_url": &lt;&lt;link to the wikipedia page of the Free Software&gt;&gt;,
                "success_case_list": [{
                        "title": &lt;&lt;title of success case&gt;&gt;,
                        "description": &lt;&lt;description of success case&gt;&gt;,
  						"image": &lt;&lt;url to screenshot of success case&gt;&gt;,
                        "industry": &lt;&lt;industry, this success case is from&gt;&gt;,
  						"customer": &lt;&lt;name of client/customer&gt;&gt;,
                        "country": &lt;&lt;country of origin of customer&gt;&gt;,
                        "language": &lt;&lt;language of success case&gt;&gt;,
                        "url": &lt;&lt;url to success case&gt;&gt;
                }, {
                        &lt;&lt;...next success case...&gt;&gt;
                }]
        }, {
          &lt;&lt;... next Free Software ...&gt;&gt;
        }]
}
</code></pre>


<h1>Software Categories</h1>
<p>
Free Software is categorized using the following terms:
</p>
<ul>
        <li>Communication (email, chat, videoconferencing, etc.)</li>
        <li>Database (SQL, NoSQL, etc.)</li>
        <li>Application (ERP, CRM, e-commerce, project management, etc.)</li>
        <li>Analytics (big data, machine learning, data visualisation, etc.)</li>
        <li>Developer (text editor, IDE, frameworks)</li>
        <li>Gis (map editor, map visualisation)</li>
        <li>Desktop (desktop operating system, desktop web browser, desktop VM, etc.)</li>
        <li>Mobile (mobile operating system, mobile web browser, mobile VM, etc.)</li>
        <li>Middleware (ESP, ETL, ELT, etc.)</li>
        <li>Infrastructure (public cloud, private cloud, software defined network, hyperconverged OS, IOT management)</li>
</ul>
<p>
The following industries are used to categorize success cases:
<p>
<ul>
  <li>Aerospace</li>
  <li>Appliances</li>
  <li>Commerce</li>
  <li>Construction</li>
  <li>Entertainment</li>
  <li>Finance</li>
  <li>Housing</li>
  <li>Insurance</li>
  <li>Life Sciences</li>
  <li>Manufacturing</li>
  <li>Media</li>
  <li>Public Administration &amp; Government</li>
  <li>Research</li>
  <li>Retail</li>
  <li>Software</li>
  <li>Telecommunication</li>
  <li>Tolling</li>
  <li>Tourism</li>
  <li>Travel</li>
  <li>Transport</li>
  <li>Web</li>
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
application is intended to be primarily persistent and communication is not. Online messaging can thus be 
considered in some cases as communication (such as SMTP email) and in other cases as application
(such as in a CRM).
</p>

