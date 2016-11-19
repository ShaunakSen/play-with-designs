Creating a custom bootstrap theme
____________________________________

Download bootstrap sass project from bootstrap website

Create scss file called app.scss

@import "../bootstrap-sass-3.3.7/assets/stylesheets/bootstrap";

//Import bootstrap-compass as well

@import "../bootstrap-sass-3.3.7/assets/stylesheets/bootstrap-compass";

Link to this file in index.html

Note: we do not need bootstrap.min.css anymore as we are already importing bootstrap in app.scss

We want to create a custom variables sass file

Create file called _customVariables.scss

Copy all code from /bootstrap-sass-3.3.7/assets/stylesheets/bootstrap/_variables.scss into this file

Then in app.scss

@import "customVariables";

Now customVariables basically contains all vars in bootstrap

So if we change any var in there it will be reflected in our project

$navbar-height:                    70px !default;

// Navbar links
$navbar-default-link-color:                #fff !default;
$navbar-default-link-hover-color:          #fff !default;
$navbar-default-link-hover-bg:             darken($navbar-default-bg, 6.5%) !default;
$navbar-default-link-active-color:         #fff !default;
$navbar-default-link-active-bg:            darken($navbar-default-bg, 6.5%) !default;
$navbar-default-link-disabled-color:       #fff !default;
$navbar-default-link-disabled-bg:          transparent !default;

Change the above values in customVariables and change will be reflected

Download fontawesome now
fontawesome/scss/ contains all sass files

Import that into our project

in app.scss:

Copy the fonts/ folder into custom-bootstrap-theme/

Now we can add icons

Now we want to add a custom scss file where we will write our own styles

Create file _custom.scss

In app.scss:

//Import custom styles

@import "custom";



