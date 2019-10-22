# disappearing-fixed-top-nav
Fixed top navigation better allows your users to navigate your site has they go through its content; however, fully fixed navigations can often take up precious real estate as a user scrolls down a page. The solution? Have a fixed navigation that only shows as a user scrolls back up.

## Tutorial		  
For detailed instruction's, view Solodev's [Build a Fixed Top Navigation that Disappears as you Scroll](https://www.solodev.com/blog/web-design/bootstrap/build-a-fixed-top-navigation-that-disappears-as-you-scroll.stml) article.
 
## Demo  		  
Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/j2wbvc9g/1/).

## HTML
The tutorial contains the following basic HTML markup.

```
 <nav class="navbar h-navbar p-0 fixed-top" role="navigation">
		<div class="container">
			<div class="row align-items-center">
				<div class="col-xl-3 col-lg-2 col-sm-4 col-5">
					<a href="/">
						<img alt="LunarXP Logo" class="img-fluid py-3" src="https://raw.githubusercontent.com/solodev/disappearing-fixed-top-nav/master/images/logo.png" aria-role="logo">
					</a>
				</div>
				<div class="col-xl-9 col-lg-10 col-sm-8 col-7">
					<ul class="navbar-nav flex-row justify-content-end flex-wrap align-items-center mr-lg-4 mr-xl-0">
						<li class="nav-item px-3 text-uppercase mb-0 position-relative d-none d-lg-flex"> <a class="d-block w-100 h-100 text-white py-4 position-relative top-link" href="#"><strong>About</strong></a>
						</li>
						<li class="nav-item px-3 text-uppercase mb-0 position-relative d-none d-lg-flex"> <a class="d-block w-100 h-100 text-white py-4 position-relative top-link" href="#"><strong>Locations</strong></a>
						</li>
						<li class="nav-item px-3 text-uppercase mb-0 position-relative d-none d-lg-flex"> <a class="d-block w-100 h-100 text-white py-4 position-relative top-link" href="#"><strong>Products</strong></a>
						</li>
						<li class="nav-item px-3 text-uppercase mb-0 position-relative d-none d-lg-flex"> <a class="d-block w-100 h-100 text-white py-4 position-relative top-link" href="#"><strong>Shop</strong></a>
						</li>
						<li class="nav-item px-3 text-uppercase my-3 my-lg-0 mr-5 mr-lg-4 mr-xl-5 d-none d-lg-flex"> <a class="d-block w-100 h-100 text-white py-4 position-relative top-link" href="#"><strong>Contact</strong></a>
						</li>
					</ul>
					<button id="sidenav-open-btn" class="menu-hamburger position-absolute pointer p-0"> <span class="icon-bar"></span>
						<span class="icon-bar"></span>
						<span class="icon-bar"></span>
					</button>
				</div>
			</div>
		</div>
	</nav>
	<section class="container pb-5" id="maincontent">
		<div class="row">
			<div class="col-md-12 col-lg-8 order-md-1 col-centered">
				<h1 class="text-center p-5 display-4">The Cosmos Awaits</h1>
				<p class="mb-4">Rogue cosmos muse about Rig Veda concept of the number one hydrogen atoms. Brain is the seed of intelligence emerged into consciousness are creatures of the cosmos the only home we've ever known hearts of the stars corpus callosum. Something incredible is waiting to be known vastness is bearable only through love vanquish the impossible vanquish the impossible the carbon in our apple pies are creatures of the cosmos.</p>
				<p class="mb-4">Hydrogen atoms extraplanetary Sea of Tranquility shores of the cosmic ocean rogue not a sunrise but a galaxyrise. A still more glorious dawn awaits finite but unbounded across the centuries invent the universe dispassionate extraterrestrial observer vanquish the impossible? Courage of our questions made in the interiors of collapsing stars white dwarf made in the interiors of collapsing stars take root and flourish vastness is bearable only through love.</p>
				<p class="mb-4">Concept of the number one billions upon billions citizens of distant epochs stirred by starlight consciousness the only home we've ever known? With pretty stories for which there's little good evidence a still more glorious dawn awaits of brilliant syntheses Sea of Tranquility Rig Veda paroxysm of global death. The sky calls to us emerged into consciousness Apollonius of Perga courage of our questions extraordinary claims require extraordinary evidence hearts of the stars and billions upon billions upon billions upon billions upon billions upon billions upon billions.</p>
				<p class="mb-4">Colonies realm of the galaxies prime number brain is the seed of intelligence network of wormholes encyclopaedia galactica. Not a sunrise but a galaxyrise cosmic fugue the ash of stellar alchemy hundreds of thousands a very small stage in a vast cosmic arena not a sunrise but a galaxyrise. Hundreds of thousands citizens of distant epochs Sea of Tranquility the carbon in our apple pies extraordinary claims require extraordinary evidence the sky calls to us.</p>
				<p class="mb-4">Apollonius of Perga citizens of distant epochs great turbulent clouds venture Euclid how far away? Encyclopaedia galactica kindling the energy hidden in matter vanquish the impossible across the centuries rings of Uranus worldlets. With pretty stories for which there's little good evidence stirred by starlight hundreds of thousands kindling the energy hidden in matter with pretty stories for which there's little good evidence vastness is bearable only through love.</p>
				<p class="mb-4">White dwarf intelligent beings shores of the cosmic ocean tingling of the spine rich in heavy atoms vastness is bearable only through love. The sky calls to us extraordinary claims require extraordinary evidence permanence of the stars trillion finite but unbounded a mote of dust suspended in a sunbeam. Dream of the mind's eye concept of the number one a mote of dust suspended in a sunbeam cosmic ocean at the edge of forever cosmic ocean?</p>
			</div>
		</div>
	</section>
	<!-- Optional JavaScript -->
	<script>
		$(window).scroll(function(e) {
		
		// add/remove class to navbar when scrolling to hide/show
		var scroll = $(window).scrollTop();
		if (scroll >= 150) {
		    $('.navbar').addClass("is-hidden");
		} else {
		    $('.navbar').removeClass("is-hidden");
		}
		
		});
	</script>
```

## External Resources
This tutorial includes the following third party resources.

```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
<!-- jQuery first, then Popper.js, then Bootstrap JS -->
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
```
