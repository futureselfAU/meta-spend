<select id="candidate-select">
  <option value="canning">Canning</option>
  <option value="curtin">Curtin</option>
  <option value="flinders">Flinders</option>
  <option value="wa-liberal">WA Liberal Candidates</option>
</select>

<div id="canning-section">
  <h1>Canning</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="948595148496917,498624823340124" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="948595148496917,498624823340124" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="curtin-section" style="display: none;">
  <h1>Curtin</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,110679918187811" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,110679918187811" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="flinders-section" style="display: none;">
  <h1>WA Liberal Candidates</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
<script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
<div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="503830579480432,103943488824397" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
<script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
<div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="503830579480432,103943488824397" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<div id="wa-liberal-section" style="display: none;">
  <h1>WA Liberal Candidates</h1>
  <h3>90 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,262340686960375,948595148496917,357223777483754,442693582252181,346201718577605,776811619361742,428271723699770,146533948886081,125627804305487" data-time-preset="last_90_days" data-width="500"></div>
  {% endraw %}
  <br>
  <br>
  <h3>7 Days</h3>
  {% raw %}
  <div id="fb-root"></div>
  <script async defer src="https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v7.0"></script>
  <div class="fb-ad-library-spend-tracker" data-country="AU" data-page-ids="289373994253840,262340686960375,948595148496917,357223777483754,442693582252181,346201718577605,776811619361742,428271723699770,146533948886081,125627804305487" data-time-preset="last_7_days" data-width="500"></div>
  {% endraw %}
  <br>
</div>

<script>
  document.getElementById("candidate-select").addEventListener("change", function() {
    var selection = this.value;
    // Hide all sections first
    document.getElementById("canning-section").style.display = "none";
    document.getElementById("curtin-section").style.display = "none";
    document.getElementById("flinders-section").style.display = "none";
    document.getElementById("wa-liberal-section").style.display = "none";
    
    // Show the selected section
    if (selection === "curtin") {
      document.getElementById("curtin-section").style.display = "block";
    } else if (selection === "wa-liberal") {
      document.getElementById("wa-liberal-section").style.display = "block";
    } else if (selection === "canning") {
      document.getElementById("canning-section").style.display = "block";
    } else if (selection === "flinders" {
      document.getElementById("flinders-section").style.display = "block";
    }
  });
</script>
