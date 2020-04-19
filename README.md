# Splunk-Workshop
Splunk is a software platform to search, analyze and visualize the machine-generated data gathered from the websites, applications, sensors, devices etc. which make up your IT infrastructure and business. Machine-generated data is often difficult to read, analyze, and organize, but Splunk allows us to do all of this and more. Like Google or Bing, you can think of Splunk is like a search engine for machine-generated data.

## Who uses Splunk?
Over 13,000 companies are currently using Splunk in a wide range of domains:
* Computer Software
* Information Technology and Services
* Financial Services
* Health Care
* Higher Education
* Government Administration
* Telecommunications
* Computer Hardware
* Retail
* Insurance

## How are they using Splunk?

### Vodafone  
![vodafone](images/vodafone.png)  
Vodafone is a telecommunication company that generates a massive amount of customer data. They use Splunk to manage their big data in order to optimize and provide better their customer support.

### Domino's Pizza
![dominos](images/dominos.png)  
Domino's utilizes Splunk to analyze customer habits to better understand their wants and behaviors.

## Getting Started

These instructions will get Splunk up and running on your local machine for development and demo purposes. 

### Installing

Create a free account and download the free Enterprise Version for the machine you are using.  
(Get 64-bit version if using Windows 10)
* [Splunk Install](https://www.splunk.com/) 

## Splunk Search and Reporting (Demo)
The Search & Reporting application (Search app) is the primary interface for using the Splunk software to run searches, save reports, and create dashboards. The application lets you search your data, create data models and pivots, save your searches and pivots as reports, configure alerts, and create dashboards, and is provided by default.

### Input Data into Splunk

In order to see how Search and Reporting works we will need some data to analyze. This data is machine-generated data from a fictional company's server system. Go to [this link](https://docs.splunk.com/Documentation/Splunk/8.0.3/SearchTutorial/Systemrequirements#Download_the_tutorial_data_files) and download the tutorialdata.zip located halfway down the page.  

![download](images/wsdatadownload.PNG) 

Next, go to the Splunk home page and select Add Data.

![addData](images/uploaddata.PNG)

Scroll to the bottom of the page and select Upload, as we want to use the data we just downloaded.  

![Upload](images/uploadSmall.png)

From here you will select the tutorial.zip file. Press the Next button, followed by Review, then finally Submit.  
We are now ready to search and analyze our new data!

### Searching the Data

Now that we have some data to analyze, let's try out Splunk's Search application.

Still, on the same page, press the Start Searching button to begin searching through the data we just uploaded. 

![Search](images/startSearchingSmall_LI.jpg)

This is the main interface for Splunk's Search and Reporting.

![firstSearch](images/firstsearchsmall.png)  

To start, let's see if there has been any 503 Service Errors. Click in the search box and clear the current text. Next, type in the following command and press enter.

```
503
```

Splunk will search through the data file for any events which relate to the keyword 503.

![503](images/error503smaller.png)

Similar to SQL, you can use special keywords such as *and, or* to refine the search.

```
buttercupgames (error OR fail* OR severe)
```

This query will return buttercupgames events that contain an erorr, types of failures, or a severe tag. 

![buttercup](images/buttercupsmall.png)

Here is a quick guide to better understand all of the information Splunk offers in the UI.

![guide](images/dataguidesmaller.png)

## Addition Resources
**If you are interested in learning more about Splunk and how to fully utilize its tools, visit** [Splunk-Fundamentals](https://www.splunk.com/en_us/training/free-courses/splunk-fundamentals-1.html) 

## Authors

* **David Curtis** - [davidbradlycurtis](https://github.com/davidbradlycurtis)  
![Portrait](images/smallthumbnail.jpeg)

## References

* https://www.edureka.co/blog/what-is-splunk/
* https://www.splunk.com/
* https://docs.splunk.com/Documentation
* https://enlyft.com/tech/products/splunk
