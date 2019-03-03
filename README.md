# Health-Tech-Depression-Webapp

We created a simple web-app that search the SMART on FHIR database for depression related condition, such as depression, depressive disorder of all levels. We pull all the patient data and aggregate their information, to create pie charts on the demographics, such as Gender and Age. Our stats aims on population level and visualize how depression-related illness breaks down demographically.

The pie chart contain more detailed information on the percentages and what each slice stands for once user hover over the slice they want to query. Data visualization and animations are done with D3.js. This is a single page application, which combines HTML, CSS and JavaScript file in one file. We use jQuery to fire request to FHIR APIs.

To run the program, simple type in "python -m SimpleHTTPServer" which will run the program on your local host. Type "localhost:8000" in your chrome browser, then you will be able to see the visualization as well as animation. The reason we use python to mimic a simple HTTP server is to avoid Cross-Origin problems in chrome, firefox, IE, etc. 

Limitations: we only have 8 patients in the database that has related illness. Given such condition, our stats is limited. However, the implementation can be applied to larger data volume as the code is as general as possible.
