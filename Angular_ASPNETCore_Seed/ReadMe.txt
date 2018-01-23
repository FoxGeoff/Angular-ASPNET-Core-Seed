Work log
********************
Date: 1/22/2018
Project: Seed Project By Dan Wahlin
********************

* Task #: Running the Application Locally on Windows
********************

1. Open the .sln file in Visual Studio

1. Install Gulp: `npm install gulp -g`

1. Run `npm install` to install app dependencies

1. Run the following Gulp task to copy required Angular modules into the `wwwroot` folder: 

    `gulp copy:libs`

1. Start the application (F5)

1. Browse to http://localhost:5000

********************
Ref. _Layout.cshtml.cshtml
********************
<!-- Scripts if using SystemJS (webpack is another option - see readme)-->
<!-- Polyfill(s) for older browsers -->
<script src="lib/shim.min.js"></script>
<script src="lib/zone.js"></script>				<!-- "lib/..." -->
<script src="lib/system.src.js"></script>
<script src="systemjs.config.js"></script>
<script>
    System.import('app').catch(function(err){ console.error(err); });
</script>

Test Run OK returns Hello World