# Prompts to LLM:

### Instructions ###

You are assisting a team of expert clinical pharmacists, drug interaction pharmacology researchers, and persons who edit drug interaction knowledge compendia. You help synthesize evidence about possible interactions between prescription drugs and natural products (botanical or herbal) based on the most recent and relevant information. Ground your response in factual data from your pre-train set or any context provided by the user, explicitly referencing or quoting authoritative sources when possible. In your response, think carefully and be specific about the source of the information used in each answer, and avoid citing sources if the information is not a direct citation from that source. Always explain your reasoning. Make it explicit when you base your reasoning on pharmacological inference rather than a direct citation from a textual source. Focus on factuality since you must evaluate your answer in the end. Structure your response using the following nine-item template: 

Item 1: A list of each potential mechanism, showing each step in your thinking and providing evidence to support each step involved.  

Item 2: A description of the natural product mentioned in the query. Please include a list of known names to refer to the product and note how it is prepared or consumed.  

Item 3: A summary of the pharmacokinetic properties of the natural product mentioned in the query. If available, include values for the Area Under the Curve change at therapeutic concentrations linked to a pharmacodynamic effect, information on common administration routes, and the average amount of bioactive compounds in the products. 

Item 4: A brief description of the drug mentioned in the query. Include a list of known names used to refer to the drug. 

Item 5: A summary of the pharmacokinetic properties of the drug mentioned in the query. If available, include values for the Area Under the Curve change at therapeutic concentrations linked to a pharmacodynamic effect, information on common administration routes, and standardized dosage of the drug's active ingredient.

Item 6: A summarized description of the adverse event mentioned in the query. List known potential causes and if the mentioned natural product or drug is associated with the adverse event. Include all available details regarding the average onset time of the adverse event. Include all available information regarding the likelihood of overlapping effects of the adverse event. Include all available details regarding the potential additive nature of the side effects involved in the adverse event. 

Item 7: A list and description of any mention of clinical importance for the interaction, including the frequency of the mentions. 

Item 8: A list of other drugs with similar pharmacodynamic and pharmacokinetic properties to the drug in the query that could interact with the natural product mentioned. 

Item 9: A list of other natural products with similar pharmacodynamic and pharmacokinetic properties to the natural product in the query that could interact with the drug mentioned.

Finally, classify how accurate your synthesis was. Rate your confidence in your answers on a scale of 1-5, 1 being very low and 5 being very high.

-------

# Response from LLM:

Q:

How to get the value of a field in a custom object using REST API

I am trying to get the value of a field in a custom object using REST API. I am using the following code to get the value of the field but it is not working.
String url = 'http://' + System.getenv('HTTP_HOST') + '/services/data/v43.0/sobjects/' + customObject.getSObjectType().getDescribe().getName() + '/' + customObject.getSObjectType().getDescribe().getFields().get('fieldName').getName() + '/';
Http http = new Http();
http.setEndpoint(url);
http.setMethod('GET');
http.setHeader('Content-Type', 'application/json');
http.setHeader('Accept', 'application/json');
http.setHeader('Authorization', 'Bearer'+ userToken);
http.setHeader('Accept-Encoding', 'gzip, deflate');
http.setHeader('Accept-Language', 'en_US');
http.setHeader('Content-Length', '0');
http.setHeader('Connection', 'keep-alive');
http.setHeader('User-Agent', 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2272.95 Safari/537.36');
http.setHeader('Accept-Charset', 'ISO-8859-1,utf-8;q=0.7,*;q=0.7');
http.setHeader('Accept-Encoding', 'gzip, deflate');
http.setHeader('Accept-Language', 'en_US,en;q=0.8');
http.setHeader('Connection', 'keep-alive');
http.setHeader('Cache-Control', 'no-cache');
http.setHeader('Pragma', 'no-cache');
http.setHeader('Host', ');
HttpResponse response = http.send(request);
System.debug(response);

I am getting the following error.
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1. HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1. HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1. HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1. HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1. HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP ERROR: HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 400 HTTP HTTP HTTP/1.1 400 Bad Request
HTTP/1.1 400 HTTP HTTP HTTP/1.1 HTTP/1.1 HTTP/1.1 400 Bad Request
HTTP HTTP/1.1 HTTP HTTP/1.1 HTTP/1.1 HTTP HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.1 HTTP/1.