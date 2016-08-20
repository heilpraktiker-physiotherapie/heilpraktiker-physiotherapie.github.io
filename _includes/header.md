<header class="site-header">
  <a href="{{ site.baseurl }}/" class="logo"><span class="logo amp-close-image hoveropacity midgrey"><amp-img src="{{ site.baseurl }}{{ site.logo }}" width="40" height="40" /></span></a>
  
   
    <nav>
         <a href="{{ site.baseurl }}/" class="logo">
           <button id="homebt">
            <amp-img src="{{ site.baseurl }}/assets/images/logosvg.svg" alt="Welcome" height="60" width="60"></amp-img>
        </button>
        </a>
        <button id="sidebartogglebutton" on="tap:sidebar.toggle" class="barbuttons">
            <amp-img src="assets/images/Burger.svg" alt="an image" layout="fixed" width="40px" height="40px"></amp-img>
        </button>
        
        <div class="navbuttonsbar right">
          {% assign sorted_pages = site.pages | sort:"name" %}
           {% for my_page in sorted_pages %}
              {% if my_page.title %}
              <a class="page-link" href="{{ my_page.url | prepend: site.baseurl }}"><button class="barbuttons">{{ my_page.title }}</button></a>
              {% endif %}
            {% endfor %}
        </div>
    </nav>
</header>
