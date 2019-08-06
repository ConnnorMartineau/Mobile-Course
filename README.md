# Mobile-Course
Mobile Application Development Course

{Documentation}
-Purpose of the site: This is my project for Professor Gary Tanner's Mobile Application Development Course at Rasmussen College.
-Site map - see the file through the sotd because github no longer has the "Launce automatic page generator"
-The site includes a homepage with links to 9 other pages on the site. These include:
	-about you- which has five different fields with three different form elements.
	-flavors- which would contain information of flavors the company sells.
	-new releases- which would contain information on all of their new products.
	-box mods- which would contain information on all of their box mods.
	-salt mods- which would contain information on all of their salt mods.
	-tournaments- which would contain information on all tournaments they have hosted and are projected to host.
	-best sellers- which contains a filtered list of their 6 best sellers, one highlighted with a standard icon.
	-about us- which would contain information about the company
	-grid- which contains two rows of 3 columns of a grid.
-There is a navigation panel that slides from the right of the screen that would allow the user to navigate to either juices, mods, or best sellers.
-The site contains 3 different swatches from ThemeRoller that alternate throughout each link.
-The site contains web storage.
-Each page of the site contains a footer with a copyright.
-The site contains a logo of the company on the homepage.
-https://connnormartineau.github.io/Mobile-Course/
{/Documentation}
	
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>jQuery Mobile Web App</title>
<meta name="viewport" content="width=device-width,initial-scale=1" />
<link rel="stylesheet" href="css/themes/project_theme.css" />
<link rel="stylesheet" href="css/themes/jquery.mobile.icons.min.css" />
<link rel="stylesheet" href="http://code.jquery.com/mobile/1.4.5/jquery.mobile.structure-1.4.5.min.css" />
<script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
<script src="http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
</head>
<body>

<div id="page" data-role="page" data-theme="a" data-add-back-btn="true">
	<div data-role="header" data-theme="a">
	  <div class="logo"><img src="images/logo.png" width="275" height="75" alt=""/></div>
	</div>

	<div data-role="panel" id="myPanel" data-display="push" data-position="right">
		<h2>Where to Next?</h2>
		<ul data-role="listview" data-theme="c">
			<li class="menu"><a href="#">Juices</a></li>
			<li class="menu"><a href="#">Mods</a></li>
			<li class="menu"><a href="#">Best Sellers</a></li>
		</ul>
	</div>
	<div data-role="header">
    <h1>Page Header</h1>
		<a href="#myPanel" class="ui-btn ui-btn-inline">Navigation</a>
  </div>

  <div data-role="header">
    <h1>Home</h1>
  </div>

	<div data-role="content">
		<ul data-role="listview" data-theme="a">
			<li><a href="#newform">Tell us about you!</a></li>
			<li><a href="#section1">Flavors</a></li>
      <li><a href="#section2">New Releases</a></li>
			<li><a href="#section3">Box Mods</a></li>
			<li><a href="#section4">Salt Mods</a></li>
			<li><a href="#section5">Tournaments</a></li>
			<li><a href="#PageThree">Best Sellers</a></li>
			<li><a href="#section6">About Us</a></li>
			<li><a href="#grid">Grid</a></li>



		</ul>
	</div>
	<div data-role="footer" data-theme="a">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div data-role="page" id="newform" data-theme="b" data-add-back-btn="true">
  <div data-role="header" data-theme="b" data-add-back-btn="true">
    <h1>Tell us about you!</h1>
  </div>
  <div data-role="content">

		<form action="form.php" method="post">
				<label for="fname">First name:</lable>
				<input type="text" name="fname" id="fname" data-clear-btn="true">
				<label for="lname">Last name:</lable>
				<input type="text" name="lname" id="lname" data-clear-btn="true">
				<label for="minit">Middle initial:</lable>
				<input type="text" name="minit" id="minit" data-clear-btn="true">
				<input type="reset" value="Reset Button">
				<input type="submit" value="Submit Button">
				<label for="flip-2">Do you like OEC?</label>
					<select name="flip-2" id="flip-2" data-role="slider">
    				<option value="off">Yes!</option>
    				<option value="on">Blue Yes!</option>
					</select>
				<fieldset data-role="controlgroup">
    			<legend>Do you agree that we are the best?</legend>
    			<label for="checkbox-2">I agree!</label>
    			<input type="checkbox" name="checkbox-2" id="checkbox-2">
				</fieldset>
		</form>


	</div>
  <div data-role="footer" data-theme="b">
    <h4>Footer</h4>
  </div>
</div>

<div id="section1" data-role="page" data-theme="c" data-add-back-btn="true">
	<div data-role="header" data-theme="c" data-add-back-btn="true">
	  <h1>Flavors</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="c">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div id="section2" data-role="page" data-theme="a" data-add-back-btn="true">
	<div data-role="header" data-theme="a" data-add-back-btn="true">
	  <h1>New Releases</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="a">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div id="section3" data-role="page" data-theme="b" data-add-back-btn="true">
	<div data-role="header" data-theme="b" data-add-back-btn="true">
	  <h1>Box Mods</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="b">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div id="section4" data-role="page" data-theme="c" data-add-back-btn="true">
	<div data-role="header" data-theme="c" data-add-back-btn="true">
	  <h1>Salt Mods</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="c">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div id="section5" data-role="page" data-theme="a" data-add-back-btn="true">
	<div data-role="header" data-theme="a" data-add-back-btn="true">
	  <h1>Tournaments</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="a">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div data-role="page" id="PageThree" data-theme="b" data-add-back-btn="true">
	<div data-role="header" data-theme="b" data-add-back-btn="true">
		<h1>Best Sellers!</h1>
	</div>
  <div data-role="content">
	  <h3>Header</h3>
		<ul data-role="listview" data-filter="true" data-filter-placeholder="Search items..." data-inset="true">
    	<li><a href="#">Item 1</a></li>
    	<li><a href="#">Item 2</a></li>
    	<li><a href="#">Item 3</a></li>
   	 	<li><a href="#">Item 4</a></li>
    	<li><a href="#"><i style='font-size:24px' class='fas'>&#xf0a3;</i> Item 5</a></li>
    	<li><a href="#">Item 6</a></li>
    </ul>
	</div>
	<div data-role="footer" data-theme="b">
		<h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div id="section6" data-role="page" data-theme="c" data-add-back-btn="true">
	<div data-role="header" data-theme="c" data-add-back-btn="true">
	  <h1>About Us</h1>
	</div>
	<div data-role="content">
	  <h3></h3>

	</div>
	<div data-role="footer" data-theme="c">
	  <h4>ProjectOEC &copy; 2019</h4>
	</div>
</div>

<div data-role="page" id="grid" data-theme="c" data-add-back-btn="true">
  <div data-role="header" data-theme="c" data-add-back-btn="true">
    <h1>Grid</h1>
  </div>
  <div data-role="content">
		<div class="ui-grid-b">
			<div class="ui-block-a"><div class="ui-bar ui-bar-a" style="height:60px">Block A</div></div>
			<div class="ui-block-b"><div class="ui-bar ui-bar-a" style="height:60px">Block B</div></div>
			<div class="ui-block-c"><div class="ui-bar ui-bar-a" style="height:60px">Block C</div></div>
			<div class="ui-block-a"><div class="ui-bar ui-bar-a" style="height:60px">Block D</div></div>
			<div class="ui-block-b"><div class="ui-bar ui-bar-a" style="height:60px">Block E</div></div>
			<div class="ui-block-c"><div class="ui-bar ui-bar-a" style="height:60px">Block F</div></div>
	</div><!-- /grid-a -->

</div>

<script>
(function() {

	var rasm = document.querySelector('.localstorage');

	function supportsLocalStorage() {
		return typeof(Storage)!== 'undefined';
	}

	if (!supportsLocalStorage()) {
		rasm.value = 'Your browser does not support localStorage.';
	} else {
		try {
			setInterval(function() {
				localStorage.setItem('autosave', rasm.value);
			}, 1000);
		} catch (e) {
			if (e == QUOTA_EXCEEDED_ERR) {
				alert('Quota exceeded!');
			}
		}
		if (localStorage.getItem('autosave')) {
			rasm.value = localStorage.getItem('autosave');
		}
		document.querySelector('.clear').onclick = function() {
			rasm.value = '';
			localStorage.removeItem('autosave');
		};
		document.querySelector('.empty').onclick = function() {
			rasm.value = '';
			localStorage.clear();
		};
	}

})();
</script>
