## PYREST

Pyrest is a sub module of Gempyp used for API Automation

### Why to use Pyrest?

With the help of Pyrest, we can automate APIs with minimal code.We have to just use tags present in xml file

### Pyrest Tags

some of them can be optional.  

1. name  :                Name tag will be used as the name of the testcase 

2. run_flag :             Value in this tag can be Y or N which specifies whether to run this testcase or  not. 

3. api :                  This tag will be used to provide a url for the api we want to test

4. method:                Methods are the ways you can use the apis like get, post, put etc.

5. body:                  Body can be considered as the content we want to send to the server.

6. headers:               Headers are the meta information about the Api.

7. expected_status_code:  After execution, API will return http status code like (404, 200, 403, 501, 201 etc). So here we will be specifying that status code.

8. pre_variables:         These are the testcase specific variables which are defined for use in testcase itself. Before the execution of the testcase 

9. key_check:            Users can specify keys to check from the response body and the pyprest will check for the following keys.

10. post_variables:       These are the variables which are defined after the execution of the testcase. Can be used for common responses. 

11. post_assertion:       This tag will be used to compare the response from the response body.   

#### Pyrest API Automation example

In pyrest_gorest_api.xml file, we automated several gorest APIs using pyrest. In the first testcase which is named as post_assertion_not_in, in this testcase we have specfied end point dynamically and the value is assigned in pre_variables tag. This testcase is a get api and in post-assertion tag, we are checking that some values are present in response or not. 
In other testcase we tested other possible scenarios with different type of APIs

#### Report Generated with above XML 

https://jewel.gemecosystem.com/#/autolytics/extent-report?s_run_id=GEMECO-API-PY_PROD_C10FFB2A-6C5A-48F8-B6C7-624EC438AA7F
