bootstrap-fullscreen-menu
================

A simple CSS fullscreen menu Bootstrap 3, using the bootstrap modal

#Demo:

  * https://duanewilson.github.io

##Requires:

  * Bootstrap (http://getbootstrap.com)
  * //maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css
  * //maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js

##Additional Features When Using

  * Font Awesome CDN (//maxcdn.bootstrapcdn.com/font-awesome/4.2.0/css/font-awesome.min.css)
  
##License:

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Bootstrap Fullscreen Menu</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://meagency.com/" property="cc:attributionName" rel="cc:attributionURL">@duanewilsonsf</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
  

##Code

###CSS CLASS
```css
	 /* FULL SCREEN MODAL STYLES
	-------------------------------------------------- */
	.fullscreen .modal-dialog {
		margin: 0 0 0 0;
		width: 100%;
		height: 100%;
		min-height: 100%;
		padding: 0;
		color: #333;
	}

	.fullscreen .modal-content {
		height: 100%;
		min-height: 100%;
		border-radius: 0;
		color: #333;
		background: rgba(255, 255, 255, 0.97);
	}

	.fullscreen .modal-body ul {
		padding: 100px 0 0 0;
		overflow: auto;
	}

	.fullscreen .modal-body li {
		padding: 10px 0 10px 0 ;
	}

	.fullscreen .modal-body a {
		color: #333;
		font-size: 300%;
	}

	@media (max-width: 480px){
		.fullscreen .modal-body ul {
			padding: 30px 0 0 0;
			overflow: auto;
		}

		.fullscreen .modal-body li {
			padding: 4px 0 4px 0 ;
		}

		.fullscreen .modal-body a {
			color: #333;
			font-size: 200%;
			text-transform: uppercase;
			font-weight: 700;
		}
	}
```

###Bootstrap Menu Replacement

####navbar-header 
```HTML
<button type="button" class="btn btn-link navbar-toggle collapsed" data-toggle="modal" data-target="#menuModal"> ... </button>
```

####modal
```HTML
	<!-- FULLSCREEN MODAL CODE (.fullscreen) -->
	<div class="modal fade fullscreen" id="menuModal"  tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
		<div class="modal-dialog">
			<div class="modal-content" style="color:#fff;">
				<div class="modal-header" style="border:0;">
						<button type="button" class="close btn btn-link" data-dismiss="modal" aria-hidden="true"><i class="fa fa-close fa-lg" style="color:#999;"></i></button>	
						<h4 class="modal-title text-center"><span class="sr-only">main navigation</span></h4>
				</div>
				<div class="modal-body text-center">
					<ul style="list-style-type:none;">
						<li><a href="#" class="big">Hello</a></li>
						<li><a href="#" class="big">A Menu Item</a></li>
						<li><a href="#" class="big">Another Item</a></li>
						<li><a href="#" class="big">This One Too!!</a></li>
						<li><a href="http://meagency.com" class="big">me.agency</a></li>
					</ul>
				</div>
			</div><!-- /.modal-content -->
		</div><!-- /.modal-dialog -->
	</div><!-- /.fullscreen -->
```
