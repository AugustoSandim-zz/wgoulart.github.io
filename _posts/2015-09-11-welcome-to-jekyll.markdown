---
layout: post
title:  "Primeiro Exemplo de post"
date:   2015-08-20 02:37:24
categories: css
---

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.


{% highlight scss %}

$base-font-family: "PT Serif", Georgia, "Times New Roman", serif;
$alter-font-family: "PT Serif", Georgia, "Times New Roman", serif;
$base-font-size:   16px;
$small-font-size:  $base-font-size * 0.87;
$base-line-height: 1.5;
$spacing-unit:     30px;

abbr {
    background-color: #eee;
    display: inline-block;
    padding: 3px;
    font-size: 13px;
    font-weight: bold;
    color: #555;
    text-shadow: 0 1px 1px rgba(255, 255, 255, 0.5);
    text-transform: uppercase;
    border-radius: 3px;
}

a {
	font-weight: inherit;
	line-height: inherit;
	color: #222;
	text-decoration: none;
	transition: all .2s ease-in-out;

	&:hover {
	    color: #000;
	}
}

h1 {
	a {
	    border-bottom: 0;
	}
}


*:hover > .anchor-link,
.anchor-link:focus {
    opacity: 1;
    -webkit-transition: color .16s linear;
    -moz-transition: color .16s linear;
    -o-transition: color .16s linear;
    transition: color .16s linear;
}

{% endhighlight %}

{% highlight html %}
	<div class="home">
	  <h1 class="page-heading">Post List</h1>
	  <ul class="post-list">
	      <li>
	        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
	        <h2>
	          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
	        </h2>
	      </li>
	  </ul>
	</div>

	<!-- component selector option list -->
	<script>    
	  (function (document, undefined) {
	    // component selector
	    document.getElementById('component-select').onchange = function() {
	      //document.location=this.options[this.selectedIndex].value;
	      var val = this.value;
	      if (val !== "") {
	        window.location = val;
	      }
	    }
	  })(document);
	</script>

{% endhighlight %}

{% highlight javascript %}

console.log('teste');
function handerActive(e){
	var el = {
		obj : value,
		obj2 : "value",
		obj3 : 'value'
	};
	el.continer = $('teste');
	e.preventDefault();
}
	
<script>    
  (function (document, undefined) {
    // component selector
    document.getElementById('component-select').onchange = function() {
      //document.location=this.options[this.selectedIndex].value;
      var val = this.value;
      if (val !== "") {
        window.location = val;
      }
    }
  })(document);

</script>


{% endhighlight %}

{% highlight ruby %}
def show
  puts "Outputting a very lo-o-o-o-o-o-o-o-o-o-o-o-o-o-o-o-ong lo-o-o-o-o-o-o-o-o-o-o-o-o-o-o-o-ong line"
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}


Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
