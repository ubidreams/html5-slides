# HTML5 Slide Template for Arrow Ubidreams

## Using the template

1. Download the template project using the 'Download' button from GitHub.
2. Create a directory for your presentation
3. Unzip the template files in _DIR/template_
4. Create _DIR/slides.html_ (you can change the name of course)
5. In the HMTL slides, load the following script: 
    <code><pre>
    &lt;!-- Load the main script, it will automaticaly load required resources -->
    &lt;script src='template/slides.js'></script>
    </pre></code>
    
6. Create the _section_ containing your slides:
    <code><pre>
    &lt;!-- Slide container, enabling the 'arrow-ubidreams' layout -->
    &lt;section class='slides layout-regular template-arrow-ubidreams'>
        <!-- Your slides go here  -->
    &lt;/section>	
    </pre></code>
		
7. Each _<article>_ created within this section is a slide

## Changing the _template_ path

If you want to customized the location of the template, you need to update the _TEMPLATE\_PATH_ variable before loading the script:

    <!-- Customize TEMPLATE_PATH -->
    <script>
        var TEMPLATE_PATH="../";
    </script>
    <script src='../slides.js'></script>

By default _TEMPLATE\_PATH is set to _template/_

## Updating the style

The style is developed with [Less](http://lesscss.org/).

1. Update the _styles.less_ file.
2. Recompile the the less file with:

	lessc styles.less > styles.css
	
