# TLinternship

Question:

In this task, your goal is to find pages from the common crawl archive that discuss or are relevant to COVID-19’s economic impact. We would like you to produce a list of 1000 pages (URL’s) from the 2020 archives that discuss or are relevant to COVID-19’s economic impact.

Approach:

In order to find a set of 1000 pages from the 2020 archives that are relevant to COVID-19, a ipython notebook has been created with required Python code that also makes use of the given script. For larger inputs, this code does substantial time to run. Future enhancements do include cutting down this run time. With ward.paths.gz as inputs in the same folder, with implementing the Python code, 
the output generated will be a list of dictionaries with  keys as month of publishing and values as URLs to pages with content relevant to COVID.
1. Initially, the warc.gz files month wise are read and then content in each URL is checked to see if it has any COVID related data using check_if_covid function. 
2. check_if_covid function reads the content from each page, converts the HTML to text using BeautifulSoup library. 
3. A set of key words i.e., all the words that correspond to COVID such as COVID, covid, CORONA, Corona, corona, pandemic and so on is defined. Then the extracted text in the above step is converted into tokens using nltk tokenizer and each of it is matched against this list.
4. If there is any match found, then the URL is added to the output dictionary, if not ignored. This iteration goes on for a thousand times and an output dictionary of URLs is generated.

Note:
I have applied for Computer Science Internship, however I got a Data Science Coding test. I have attempted to finish the task, with my best ability. However, I must add that this did help me learn new things in the field. 
