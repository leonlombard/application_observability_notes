# API Monitoring

API monitoring checks to see if API resources are available, working properly and responding to calls.

## What should be tracked?

**Availability:** Checks to see if the resources are avaialble, working properly and responding to calls. It can be extended to monitor availability of dependant external resources. It should alert staff so that any resources can be fixed timeously.

**Performance:** Assists in determining if the application performance is up to standard. What are the response times? Are the response times degrading? Should alert to a drop below accetable performance levels so an investigation can be performed and a solution implemented.

**Data validation:** Makes sure that the data or data format is correct. Even though the response may indicate success the application should be providing expected data according to the specification.

**Integrations:** Any integrations to 3rd party API or applications need to be monitored as these affect the underlying application APIs.

**Feature changes:** Any changes made to an API should not affect the functionality of existing APIs. However, missed existing requirements and bugs that are introduced could affect the operation of these APIs. Monitoring will assist with detection of any regression in their funcationality.

**Security:** By nature APIs introduce an application to more actors that interact with the application. It is therefore important to ensure the security requirements are met. Changes in configuration, activity of authentication requests, etc assist in detecting any potential changes to the security

## What metrics can be used to monitor APIs?

**Availablity or uptime:** This is a measure of the total time an API has been available. A typical target would be something like 99%, 99.9% or 99.99%. Depending on your monitoring needs you can monitor the downtime instead of the uptime.

**Error rate:** Errors are to be expected. However, if many of them are occurring it may indicate a problem and require an investigation. A deceded upon error rate should be decided upon and anything above that should then be investigated and fixed.

**API Consumption:** This provides a value that show that amount of requests that have been requested in a given amount of time. These are typically names as requestes per minute, request per second or queries per second. A spike in values may assist in alerting that the API is not operating in an expected manner.

**Response time or latency:** How long does an API typically take to provide the response. Each type of request may have different expected response times. However, there should still be an expected average for each API endpoint. These can be monitored and indicate when an underlying software service or server hardware is no longer operating within expectecd parameters.

## References

- [API Monitoring: A Complete Introduction](https://www.splunk.com/en_us/blog/learn/api-monitoring.html) by Splunk

## Additional Resources

- [API Performancde Monitoring](https://www.catchpoint.com/api-monitoring-tools/api-performance-monitoring) by Catchpoint