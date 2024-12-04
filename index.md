---
layout: default
title: Home
---

<h1>Welcome to My Portfolio</h1>
<p>This is my awesome portfolio site!</p>

<h2>About Me</h2>
<p>I have experience in [your skills].</p>

<h2> Areas of Interest </h2>
<ul> 
    <li>Data Analytics</li>
    <li>Model Finetuning and Deploment</li>
    <li>Economics and Finance</li>
</ul>
<h2>Skills</h2>
<ul>
    <li>Skill 1</li>
    <li>Skill 2</li>
    <li>Skill 3</li>
</ul>

<h2>Contact</h2>
<p>You can reach me at brendancopps@gmail.com</p>

<div class="tab">
    <button class="tablinks" onclick="openTab(event, 'Resume')" id="defaultopen">Resume</button>
    <button class="tablinks" onclick="openTab(event, 'Projects')">Projects</button>
</div>

<div id="Resume" class="tabcontent">
    <h1>My Resume</h1>
    <p>Content for your resume goes here.</p>
</div>

<div id="Projects" class="tabcontent">
    <h1>My Projects</h1>
    <p>Content for your projects goes here.</p>
    <a href="ames_housing.md">Ames Housing Data</a>
    [Ames Housing Project](ames_housing.md)
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
