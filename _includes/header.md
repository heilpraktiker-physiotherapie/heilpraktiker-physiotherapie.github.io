<header class="site-header">
    <nav>
        <div class="green" id="topline"/>
         <a href="{{site.baseurl}}/" class="logo">
           <button id="homebt">
            <amp-img src="{{site.baseurl}}/assets/images/LogoHPPT.svg" alt="Welcome" height="60" width="60" layout="responsive"></amp-img>
        </button>
        </a>
        <button id="sidebartogglebutton" on="tap:sidebar.toggle" class="barbuttons">
            <amp-img src="{{site.baseurl}}/assets/images/Burger.svg" alt="an image" layout="fixed" width="40px" height="36px"></amp-img>
        </button>
        <div class="navbuttonsbar right">
              <a class="page-link" href="{{site.baseurl}}/termine-und-anmeldung/"><button class="barbuttons">Termine</button></a>
              <a class="page-link" href="{{site.baseurl}}/die-fortbildung/"><button class="barbuttons">Fortbildung</button></a>
              <a class="page-link" href="{{site.baseurl}}/voraussetzungen-und-anerkennung/"><button class="barbuttons">Voraussetzungen</button></a>
              <a class="page-link" href="{{site.baseurl}}/hp-physio/"><button class="barbuttons">Infos zum HP Physio</button></a>
              <a class="page-link" href="{{site.baseurl}}/kontakt/"><button class="barbuttons">Kontakt</button></a>
              <a class="page-link" href="{{site.baseurl}}/blog/"><button class="barbuttons">Blog</button></a>
              <a class="page-link" href="{{site.baseurl}}/downloads/"><button class="barbuttons">Downloads</button></a>
        </div>
    </nav>
    <amp-sidebar id="sidebar" layout="nodisplay" side="right">
        <amp-img class="amp-close-image hoveropacity midgrey" src="{{site.baseurl}}/assets/images/closeX.svg" width="40" height="40" alt="close sidebar" on="tap:sidebar.toggle" role="button" tabindex="0"></amp-img>
          <ul>
              <li><a class="page-link" href="{{ site.baseurl }}/termine-und-anmeldung/"><button class="barbuttons">Termine</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/die-fortbildung/"><button class="barbuttons">Die Fortbildung</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/voraussetzungen-und-anerkennung/"><button class="barbuttons">Voraussetzungen</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/hp-physio/"><button class="barbuttons">Infos zum HP Physio</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/kontakt/"><button class="barbuttons">Kontakt</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/blog/"><button class="barbuttons">Blog</button></a></li>
              <li><a class="page-link" href="{{ site.baseurl }}/downloads/"><button class="barbuttons">Downloads</button></a></li>
            </ul>

    </amp-sidebar>
</header>
