# Microservices based Serverless Application deployed to IBM Cloud Engine using CLI

# Create Apps
ibmcloud ce application create --name prodlist --image us.icr.io/${SN_ICR_NAMESPACE}/prodlist --registry-secret icr-secret --port 5000 --build-context-dir products_list --build-source https://github.com/ibm-developer-skills-network/dealer_evaluation_backend.git

### Example URL: https://prodlist.1sv186ep1he5.us-south.codeengine.appdomain.cloud



ibmcloud ce application create --name dealerdetails1 --image us.icr.io/${SN_ICR_NAMESPACE}/dealerdetails --registry-secret icr-secret --port 8080 --build-context-dir dealer_details --build-source https://github.com/ibm-developer-skills-network/dealer_evaluation_backend.git

### Example URL: https://dealerdetails1.1sv186ep1he5.us-south.codeengine.appdomain.cloud



ibmcloud ce application create --name frontend --image us.icr.io/${SN_ICR_NAMESPACE}/frontend --registry-secret icr-secret --port 5001 --build-source .


### Example URL: https://frontend.1sv186ep1he5.us-south.codeengine.appdomain.cloud



# To Update:

ibmcloud ce application update --name prodlist --image us.icr.io/${SN_ICR_NAMESPACE}/prodlist --registry-secret icr-secret --port 5000 --build-context-dir products_list --build-source https://github.com/ibm-developer-skills-network/dealer_evaluation_backend.git


ibmcloud ce application update --name dealerdetails1 --image us.icr.io/${SN_ICR_NAMESPACE}/dealerdetails --registry-secret icr-secret --port 8080 --build-context-dir dealer_details --build-source https://github.com/ibm-developer-skills-network/dealer_evaluation_backend.git

ibmcloud ce application update --name frontend --image us.icr.io/${SN_ICR_NAMESPACE}/frontend --registry-secret icr-secret --port 5001 --build-source .


# Screenshots:
-------------
<img width="1280" alt="homepage" src="https://github.com/user-attachments/assets/a858aaff-beb4-47f8-837f-bf1c9edf9fda" />

<img width="1486" alt="product_dealer" src="https://github.com/user-attachments/assets/e36248e4-b150-42d5-8fa8-0db36fc2e509" />

<img width="1172" alt="product_dealer_price" src="https://github.com/user-attachments/assets/8c3ca59d-a4d7-4a24-8a87-5207a8f5b51f" />

<img width="1006" alt="product_all_dealers_prices" src="https://github.com/user-attachments/assets/cd34f7a3-5fe9-495a-88a0-7a888183bd22" />


