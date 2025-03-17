---
layout: default
title: Home
---

<h1>Welcome to My Portfolio!</h1>
<p>I'm Brendan Coppinger, a data scientist with six years of experience in finance, economics, and government. My passion lies in uncovering the stories within data and leveraging machine learning to drive impactful insights. Explore my projects to see how I've helped organizations transform their data into actionable strategies.</p>

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
    <button class="tablinks" onclick="openTab(event, 'Resume')" id="defaultOpen">Resume</button>
    <button class="tablinks" onclick="openTab(event, 'Projects')">Projects</button>
</div>

<div id="Resume" class="tabcontent">
    <h1>My Resume</h1>
    <p> Coalition Greenwich | New York, NY | Data Science Manager | March 2021 – November 2023 </p>
    <ul>
        <li>Redesigned legacy models to fit within our modern tech stack as part of a company-wide digital shift and worked with management to ensure a seamless transition between different product generations.</li>
        <li>Crafted ETL pipelines using SQL, R, Python and MATLAB to speed up data processing, maintain data quality, and shift work away from analysts. Processing shrunk from weeks to hours, allowing analysts more time to interface with their existing clients and scaling up the number of clients each analyst could effectively serve.</li>
        <li>Led a team of data scientists in developing NLP-based entity resolution algorithms that allowed us to identify matching records between datasets and efficiently integrate third-party data across our application suite.</li>
        <li>Provided feedback on prototypes, led code reviews, instituted best practices in automatic testing and version tracking, and worked with management, sales, and our clients to establish and maintain expectations about model progress and development.</li>
    </ul>
    <p> Greenwich Associates | Stamford, CT | Data Scientist | July 2018 – March 2021 </p>
    <ul>
        <li>Led the development and maintenance of all models under the Greenwich umbrella, with a focus on time series regression, XGBoost classification and regression, ElasticSearch, and soft TF-IDF models.</li>
        <li>Sourced new datasets, cleaned data, and implemented advanced feature engineering techniques. </li>
        <li>Improved model interpretability using SHAP values and relative importance metrics and presented conclusions directly to clients.</li>
        <li>Developed VBA macros to automate dashboard and PowerPoint creation, collectively saving over 100 analyst hours per quarter.</li>
    </ul>
</div>

<div id="Projects" class="tabcontent">
    <h1>My Projects</h1>
    <p>Here are a few projects that can detail the work I can produce as a Data Scientist.</p>
    <ul>
        <li><a href = "ames_housing.html">Ames Housing Project</a>: Use the popular Ames housing dataset to answer a couple of questions about neighborhoods, rising rents, and the most valuable features of a property. </li>
        <li><a href = "netflix_viewership.html">Netflix Viewerhship Project</a>: Use the small amount of publicly available data to analyze viewership data and trends and make early predictions for popular TV shows. </li>
        <li>Third Portfolio Project: To be revealed when completed.</li>
    </ul>
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
