# TDSProject1
For Utilising Github API to identify Stockholm users with more than 100 followers
#### Approach for Data Scraping
### Step 1
<ol>
<li>I used GITHUB API token for scraping the data.</li>
<li>After that utilisied requests library to extract basic filtered data using the API token</li>
<li style="color:red">"location:Stockholm followers:>100"</li>
<li>I extracted the raw json that contains the url of the repo of each user</li>
<li>Then each url of the user is passed and specific information is collected</li>
<li>While extracting the user info there  was a link to each repo using that extracted all the latest 500 repos</li>
<li style="color:red">Using params={'per_page': 100, 'page': page, 'sort': 'pushed', 'direction': 'desc'}</li>
<li> Then look for 500 pages and exteacted all the details from the repo</li>
<li> The data then was pushed to the repo</li>
</ol>

#### Interesting Insights from the data
<li> The most interesting insight was that mosre repos were pushed during office hours than non office hours</li>
<img src=OfficeHours.png></img>

### Ways to increase followers

<li> On further analysis I found out that to increase followers, it is evident that most of the repos should be pushed between 3pm to 7pm</li>

<img src=Timeday.png></img>

<h4>For more details go through <a href=https://github.com/gyanesh-iitmiimb/TDSProject1/blob/main/TDS_assignment.ipynb>Notebook Link</a></h4>

<h3>Thank You!!!</h3>

