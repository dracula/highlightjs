### [Highlight.js](https://highlightjs.org/)

#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

    git clone https://github.com/dracula/highlightjs.git

#### Install manually

Download using the [GitHub .zip download](https://github.com/dracula/highlightjs/archive/master.zip) option and unzip them.

#### Activating theme

1\. Copy `dracula.css` to your desired directory.

2\. Include the theme in your html. `<link rel="stylesheet" href="dracula.css">`

In the end, your page should look something like this:

    <link rel="stylesheet" href="dracula.css">
    <script src="http://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.4.0/highlight.min.js"></script>
    <script>hljs.initHighlightingOnLoad();</script>
    <pre><code class="javascript">
    // Scary function
    function scare(who) {
      console.log(who, 'your blood is mine');
    }
    </code></pre>
