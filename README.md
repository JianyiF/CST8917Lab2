# CST8917Lab2

## Running the app locally
create a storage account
![image](https://github.com/user-attachments/assets/c5a77312-9c91-48c0-81b1-665f97246f76)
create an azure AI foundry
![image](https://github.com/user-attachments/assets/4e4a37fe-1f45-40f3-9a22-c941fef5afd8)
create an azure open ai
![image](https://github.com/user-attachments/assets/2ede89da-42d2-4eed-ae69-4bf971da0667)
create gpt 4.1 for text complete
![image](https://github.com/user-attachments/assets/e96e7140-a23e-4c24-a96a-912b9930870d)
create form recongnizer
![image](https://github.com/user-attachments/assets/a9a5ed19-ed5b-4471-bcbd-246373615747)

clone the repo from Intelligent PDF Summarizer, and create a ``local.settings.json`` file to store all endpoints and keys from Azure portal.
install all Requirements by running:
```bash
python3 -m pip install -r requirements.txt
```
create storage input and output container for pdf summarized in durable function.
![image](https://github.com/user-attachments/assets/f5caca49-83b7-45bc-9aeb-68781c07e97f)
Start the Function App locally by running:
```bash
func start --verbose
```
![image](https://github.com/user-attachments/assets/93d04a7d-490c-495b-b015-986384423ff2)
Now uploads PDF into the ``input`` container in storage account, and after finished the orchestration, the summarized pdf should be showned in ``output`` contianer.
Since my local files got reject, i could not see the pdf been summarized and shown in ``output`` container.
![image](https://github.com/user-attachments/assets/b01c90c5-c28d-4bb8-aa74-7b2b60377c0c)


## Deploy the app to Azure
Download Azure Developer CLI(azd) and run the command to provision and deploy the app:
```bash
azd up
```
once the azd up finishes, the app should be deployed.
Since i still have the openai issue with gpt 4.1 permission issue, i could not get it working, so my demo video can only explain what i did.
![image](https://github.com/user-attachments/assets/2f3ba723-be44-48c5-98e2-c60a30ded958)

## Demo video link
https://youtu.be/u_sL7esd1j8
