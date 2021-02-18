# SAP BusinessPartners OData Mock

This provides a simle OData endpoint of the SAP BusinessPartners API with support for simple operations based on the project example project [here](https://github.com/SAP/cloud-s4-sdk-book), with a Dockerfile and easy deployment to Cloud Run.

# Deployment

To deploy either clone and build the docker image yourself, or just click this button to deploy directly to [Google Cloud Run](https://cloud.google.com/run).

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)

# Test

To test your deployment simply run this command to do a GET and return 5 test data records with the endpoint returned by the deployment above.

`curl [YOUR_CLOUDRUN_ENDPOINT]/sap/opu/odata/sap/API_BUSINESS_PARTNER/A_BusinessPartner`

You should get a lot of BusinessPartner returned.  You can also POST new records to the endpoint, which will be persisted in memory until the Cloud Run instance is scaled down.