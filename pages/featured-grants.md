---
title: Featured Grants
layout: about
permalink: /featured-grants.html
---

## Featured Grants

Lorem ipsum odor amet, consectetuer adipiscing elit. Aptent cursus consequat aptent sem ad dui erat lacus natoque. Cursus imperdiet porta massa porttitor venenatis semper. Aliquet placerat etiam tincidunt ornare et per. Facilisis rhoncus primis curae curae ante justo aptent etiam. Dis id nec pharetra primis non natoque. Blandit tempor mollis integer aenean rhoncus enim lorem? Elit taciti augue scelerisque, turpis arcu leo pretium faucibus? Vulputate ac odio mus ornare proin inceptos commodo.

I don't know if this will work but let's try it.

<div class="lefty">
<p class="featured">
<span id="grant_name" class="ref" 
          data-google-sheet-column='5' 
          data-google-sheet-row='7' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span></p>
	  <div class="darkcard">
<p>
<span id="grant_dates" class="ref" 
          data-google-sheet-column='5' 
          data-google-sheet-row='8' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span>
<br>
<span id="grant_funding" class="ref" 
          data-google-sheet-column='6' 
          data-google-sheet-row='8' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span>
<br>
<span id="grant_topics" class="ref-little" 
          data-google-sheet-column='5' 
          data-google-sheet-row='9' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span>
<br>
<span id="grant_formats" class="ref-little" 
          data-google-sheet-column='6' 
          data-google-sheet-row='9' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span>
<br>
<span id="grant_closedate" class="ref-little" 
          data-google-sheet-column='5' 
          data-google-sheet-row='10' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span></p>
<p>
<span id="grant_description" class="ref-little" 
          data-google-sheet-column='5' 
          data-google-sheet-row='11' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span> 
<br>
<span id="grant_url" class="ref-little" 
          data-google-sheet-column='6' 
          data-google-sheet-row='11' 
          data-google-sheet-url='https://docs.google.com/spreadsheets/d/e/2PACX-1vRh3494sDK_OMzGcz27h7-nDP2zGhIWCRQLDv8chKakq9nQluqxslTF17QVCfoNgqhxWTV4t2tFdELO/pub?gid=74031093&single=true&output=csv'></span>
    </p> </div>

<div id='google-sheet-replacer'>
      <script type='text/javascript'>
        // Borrowed from https://www.bennadel.com/blog/1504-ask-ben-parsing-csv-strings-with-javascript-exec-regular-expression-command.htm and minified for copy-ability reasons
        // Mod version borrowed by me from Matt Kahl via https://codepen.io/mattkahl/pen/mqGWZg
        var CSVToArray = function CSVToArray(e,r){r=r||",";for(var n=new RegExp("(\\"+r+'|\\r?\\n|\\r|^)(?:"([^"]*(?:""[^"]*)*)"|([^"\\'+r+"\\r\\n]*))","gi"),g=[[]],l=null;l=n.exec(e);){var a=l[1];if(a.length&&a!=r&&g.push([]),l[2])p=l[2].replace(new RegExp('""',"g"),'"');else var p=l[3];g[g.length-1].push(p)}return g}      
        var fetchGoogleSheetAsArray = function fetchGoogleSheetAsArray(googleSheetURL, callback) {
          var googleSheetRequest = new XMLHttpRequest();
          googleSheetRequest.addEventListener('load', function() {
            var rawCSVText = googleSheetRequest.responseText;          
            callback(CSVToArray(rawCSVText));
          });
          googleSheetRequest.addEventListener('error', function() {
            console.error('Google Sheet Replacer had trouble fetching the Google Sheet at: ' + googleSheetURL);
          })
          googleSheetRequest.open('GET', googleSheetURL);
          googleSheetRequest.send();
        }
        var processAllGoogleSheetReplacerElements = function processAllGoogleSheetReplacerElements() {
          googleSheetElements = document.querySelectorAll('[data-google-sheet-url]');
          googleSheetElements.forEach(function (googleSheetElement){
            var googleSheetURL = googleSheetElement.getAttribute('data-google-sheet-url');
            var googleSheetColumn = parseInt(googleSheetElement.getAttribute('data-google-sheet-column'), 10);
            var googleSheetRow = parseInt(googleSheetElement.getAttribute('data-google-sheet-row'), 10);
            fetchGoogleSheetAsArray(googleSheetURL, function(googleSheetArray) {
              googleSheetElement.innerHTML = googleSheetArray[googleSheetRow - 1][googleSheetColumn - 1];
            });
          });
        }
        processAllGoogleSheetReplacerElements();
      </script>
    </div>
