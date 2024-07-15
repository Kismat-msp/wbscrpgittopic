# Top Repositories for Github Topics

![Screenshot 2024-07-15 111927](https://github.com/user-attachments/assets/2b1dc556-7868-49d0-b147-73ae484c15a6)

Web scraping is the automated process of extracting data from websites. It involves using software tools to access, collect, and organize information from web pages for various purposes, such as analysis, research, or application development. Follow these step to build a web scraping project from scratch using python and it's ecosystem of libraries.

### Pick a website and describe your objective
- Browse through different sites and pick on to scrape. Check the "Project Ideas" section for inspiration.
- Identify the information you'd like to scrape from the site. Decide the format of the output CSV file.
- Summarize your project idea and outline your strategy in a Juptyer notebook. Use the "New" button above.

### Project Outline
- we're going to scrape https://github.com/topics
- we'll get a list of topic. For each topic title, topic page URL and topic description 
- for each topic, we'll get the top 20 repositories in the topic from the topic page 
- for each repository, we'll grab the repo name, username, star and repo URL
- for each topic we'll create a CSV file in the following format:

```
Repo Name,Username,Stars,Repo URL
three.js,mrdoob,98800,https://github.com/mrdoob/three.js
libgdx,libgdx,22700,https://github.com/libgdx/libgdx

```
### Use the requests library to download web pages

- Inspect the website's HTML source and identify the right URLs to download.
- Download and save web pages locally using the requests library.
- Create a function to automate downloading for different topics/search queries.

### Use Beautiful Soup to parse and extract information

- Parse and explore the structure of downloaded web pages using Beautiful soup.
- Use the right properties and methods to extract the required information.
- Create functions to extract from the page into lists and dictionaries.
- (Optional) Use a REST API to acquire additional information if required.
