# Impledge_QA_Loveleen_Batra.postman_collection
# Overview
This Postman collection is designed to test and verify API endpoints provided by EasyPost for address verification and shipment details. The collection includes multiple requests with associated test scripts to validate the functionality and correctness of API responses. The focus of this program is to ensure the API behaves as expected under various scenarios while adhering to defined test cases.
It Include 3 Test Cases
# Material Provided
A json "Impledge_QA_Exercise.postman_collection.json"file in which we have to do the changes 
# Design Decisions  
          -Address Verification:A POST request is used to verify the delivery details of an address. Test scripts are included to validate:
                                --The response body contains no errors.
                                --The ZIP code in the response matches the expected value (06810).
          -Get Shipment Details: A GET request is used to fetch shipment details using a specific ShipmentId. Test scripts are added to verify:
                                --The response returns the correct ShipmentId.
                                --The value of selected_rate.retail_rate equals 12.
                                --The retail_rate is greater than list_rate.
# Approach
  ### Reusability and Modularity:
        -Each request is self-contained, with relevant headers, authentication, and test scripts bundled together.
        -Tests are written in JavaScript within Postman to ensure they are easy to understand and extend.
  ### Validation of Business Logic:
        -Test cases explicitly validate specific fields (e.g., retail_rate, list_rate) critical to the API's purpose.
        -Logical comparisons ensure the system's output adheres to real-world expectations.
  ### Error Prevention and Debugging:
        -Tests include assertions for API status codes, ensuring the server responds correctly.
        -Meaningful messages in test scripts provide clear insight into failure points during debugging.
# Output 
      -Fix the failing test cases.
      -Add a new request to this collection to fetch details of ShipmentId
      -Verify that value of selected_rate. retail_rate is equals to 12
      -Verify that retail_rate is greater than list_rate
