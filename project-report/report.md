# A Cloud Computing Approach to Financial Decision Automation :hand: fa18-523-63

:o: please see sample for format

:o: we prefer you produce a snapshot rather than doing a proposal.

# An introduction to the project

For my project, I will be using scikit learning heavily. I intend to create several different virtual machiens that will each perform a different machine learning tool on different datasets related to financial analytics. My goal is to improve my current model using cloud computing technologies. The reason behind needing the virtual machines for this is a cosmetic need, for the sake of learning some cloud computing characterstics and intricaces for both my education and my professional career and life. One virtual machine will be used to collect daily data and statistical reports using either Yahoo's or Google's APIs for financial data on the New York Stock Exchange. Other machines will poll this data either of scp, ssh, or some other connection protocol of my choosing, and perform initial analyses, looking for correlation between the different features of the data. This will range from basic statistical analyses of the correlation of the variables to more in depth of finding correlations of the outcomes of the different machine learning algorithms. It will be recursive in nature and test it's estimations across the different days of data. Another machine will be pulling more realtime data using realtime stock, a python library for just this purpose. This would be ideal for day-traders and and more immediate decision making. A third machine will be webscraping for relevant news on a stock market ticker and its competitors to see whether that has any impact on the outcome. One machine will be running a SQL database storing the data collected by the other machines. Lastly, there will be a machine dedicated to each different machine learning algorithm, as there will be a lot of big data to sort and sift through.

# Hardware needed

I will utilize tools such as virtual box to implement this. I have a personal computer with the spefications that I believe will be able to handle the daily load in approximately 4 hours of runtime (but time will tell). The virtual machine that will need the most disk space will be the one running the SQL database. The others will need high amounts of memory, which should not be an issue for my PC that has 32 GB of internal memory with 500 GB of flash storage space if it is insufficient.

# Software needed

I will likely be running my implementations at night, reducing the need for monitoring. Scikit will be used heavily in each virtual machine as that is the major workhorse for the analytics of the project. I will write code independantally on linux (likely Xubuntu boxes) which should give ease of reproduction and implementation.

# Expected challenges

There are many expected challenges and I anticipate that I underestimate the difficulty of many aspects of this project. Firstly, I don't have a storage area network designed specifically for my data needs. I do not expect to exceed 500 GB of data used but if I do then I believe that I have the means to procure the appropriate resources for this project. 

+ Computing resouces: I haven't yet done thorough enough analyses to understand all of the CPU/GPU power that will be required for this project. I do have a healthy and stable CPU which I believe will help, but time will tell whether it will be sufficient for my needs.
+ Memory resources. I don't expect to exceed the 32 GB of memory that I have procured and I do have a healthy amount of flash storage which should serve as a capable backup, resulting in minimal overhead when it comes to computing time. I will only be using spinning disks for the SQL database but I have not yet decided whether I will make this RAID protected or not.
+ Storage resources: as mentioned earlier, I will not have access to a full storage area network and the potential exists for exceeding the disk capactiy that I have available for this project. This is a minimal fear as prelimary tests didn't use more than 100 GB of data, which was easily handled byh one of my solids state drives.
+ I anticipate that I understimate the difficulty of the communcation between the different virtual machines. I am doing it in the way that I am to make this a learning opportunity. I know that this will add overhead but it is expected to be joyous overhead designed with the purposes of learning the domain private cloud computing.
+ Implemenation of the machine learning algorithms will be a little difficult as I only consider myself an expert in about 4 different algorithms, the ones that I know how to code from scratch. For ther others, I will be using scikit-learn for that express purpose, to ease the implemenation.
+ I expect that I will run into some networking issues despite it all being hosted on a singular machine. I will need to carefully define IP addresses or devise names to mitigate this communication issue and ensure that all of the proper TCP ports will be open for the communication to occur between my storage nodes, my analytic nodes, and my results nodes.

# Project Hypotheses

+ I conject that I will be able to improve my currently used model for my automate robo-advising tools by nearly 30% of the growth. This modest prediction is likely to occur because I will be using more sophisticated machine learning tools and I will not be overutilizing a single program at once (as multithreaded as my previous code may be). 
+ I hypothesize that this method will have 40% less overhead than my previous method as multiple algorithms will be able to run simultaneously and the different algorithms will be independent of eachother.

# The end goal

The end goal will be a final machine learning clustering algorithm to assign to one of five categories for each stock type: strong sell, weak sell, neutral, weak buy, strong buy. The only stocks that I intend to own are those that will result in the strong buy category and I intend to refuse to own any that show up in the strong sell category. I believe that this heavy use of machine learning will prove to be an effective improvement on my currently used models and will result in the model that I will use in the future, minus many of the overheads of the virtual machines.
