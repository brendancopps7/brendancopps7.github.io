---
layout: default
title: Home
---
<h1> Ames Housing Project </h1>
<p> I wanted a project on my portfolio that was similar to the Phialdephia Housing Index, which I worked on in my time with Econsult Solutions.</p>
<p> Unfortunately it looks like the housing index hasn't been updated with new data since 2021.</p>

<p> The Ames Housing Dataset available in R has similar datapoints to the data we worked with internally, so let's see if we can recreate those shiny apps here.</p>

<p> A couple of guiding questions: </p>
<ul>
    <li>How can we define neighborhoods in Ames, Iowa?</li>
    <li>What is the best time of year to buy a house?</li>
    <li>Where is the best place to purchase a house in Ames?</li>
</ul>
<div class="tab">
    <button class="tablinks" onclick="openTab(event, 'Results')" id="defaultOpen">Results</button>
    <button class="tablinks" onclick="openTab(event, 'Process')">Process</button>
</div>
<div id="Results" class="tabcontent">
    <h1>Final Results</h1>
    <h2>How can we define neighborhoods in Ames, Iowa</h2>
    <p>The dataset gives us the info we need</p>
    <h2>What is the best time of year to buy a house?</h2>
    <p>Given an ever increasing housing market, probably the beginning of the year</p>
    <h2>Where is the best place to purchase a house in Ames?</h2>
    <p>Wherever you want to live really</p>
</div>

<div id="Process" class="tabcontent">
    <h1>My Projects</h1>
    <p>Content for your projects goes here.</p>
    This is gonna be the space where I have the code that creates the project
</div>
<script>
//Create two tabs to flip between resume and project views
function openTab(evt, tabName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(tabName).style.display = "block";
    evt.currentTarget.className += " active";
}
// Automatically click the default tab 
document.getElementById("defaultOpen").click();
</script>


<style>
.tab {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
}

.tab button {
    background-color: inherit;
    border: none;
    color: black;
    cursor: pointer;
    padding: 10px 20px;
    font-size: 16px;
}

.tab button:hover {
    background-color: #ddd;
}

.tab button.active {
    background-color: #ccc;
}

.tabcontent {
    display: none;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
}
</style>
