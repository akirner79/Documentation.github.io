## MBM API Overview<br>

### Requests<br>
The MBM APIs are based on REST principles. Data resources are accessed via standard HTTPS requests to an API endpoint.

|**METHOD**|**ACTION**|
|:------:|------|
|GET|Retrieves Resouces|
|POST|Creates Resources|
|PUT|Changes and or replaces resources or collections|
|DELETE|Deletes resources|

### Pagination
Some endpoints allow a way of paging the dataset requested. This is can be done by taking an ```offset``` and ```limit``` as part of the query parameters. ```offset``` is index based, so the beginning of the list starts at 0.

Example of pagination here something like ```[api.mbm.com/v123/workqueue/assignments?assignmentType=Ownership&offset=20&limit=100]```
<br><br>
### **HTTPS Response Codes**<br>
The listed response codes are possible for the MBM Workqueue API. For further information, see [HTTPS Response Status Codes](https://www.google.com).
|STATUS CODE|DECSRIPTION|
|:-----:|-----|
|200|OK- The request has succeeded. The information returned witht he repsonse is dependant on the method used in the request.|
|500| Internal Server Error. The server has encountered a situation it doesnt know how to handle.|
|XXX| This is the master list of all HTTPS Repsonse codes we support|


### **Application Response Codes**<br>
The listed response codes are possible for the MBM Workqueue API. For further information, see [Application Response Status Codes](https://www.google.com).
|STATUS CODE|DECSRIPTION|
|:-----:|-----|
|123|A new authorization cannot be submitted until authorization ```hscid``` is completed.|
|124|The following duplicate authorizations have been found.```hscid``` ```hscid``` ```hscid``` ```hscid``` |
|XXX| This is the master list of all HTTPS Repsonse codes we support|

