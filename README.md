**Virtual Shopping Assistant**
-------
##**Contributors**
- Prashant Mishra (prashant24.juit@gmail.com)
- Geetanjli Chugh (geetanjli015@gmail.com)
- Sneh Pahilwani (snehpahilwani@gmail.com)
- Yash Sinha (yash.sinha08@gmail.com)

##**Architecture**
![Alt text](/images/flowchart.png?raw=true "Optional Title")

##**Description**
The aim of this app is to improve the user experience and decrease the time spent while shopping online. We have built an adaptive and interactive Android-based virtual salesman application which will try to address this concern. The agent will be able to assist the user while shopping and will filter the options based on user’s requirements to show a focused list of products for the user to choose from.

The application is developed using Android SDK and API.AI SDK with SQLite as the database in backend. 
- The frontend is developed on Android SDK with a list view displaying segregated product items. Each item consists of name, price, image and a unique product number.  
- The product data has been scraped from Amazon with attributes like size, gender, color, brand etc. and added to the static database. This database contains 287 unique products. 
- The application uses the API.AI SDK for ASR and NLU. The ASR is built using Android’s SpeechRecognizer() with API.AI’s ASR layer. The possible utterances and variables for each action and context are written manually on API.AI’s console. API.AI handles the resolution of a query. The dialogue manager is built in the APIAITaskAgent class. This class acts as the controller of the framework, which receives voice input from the user, sends it to API.AI and obtains the resolved query. The agent then triggers different queries and responses based on the context of the dialogue and response by the user.
- The database is queried by the Dialogue manager and then an appropriate response is given to the user by the Android’s TTS.
- Concurrently, the results are shown on the home page and the filters are dynamically updated on the front page

##**Screenshots**
 ![](/images/screen1.png?width=200)    ![](/images/screen2.png?width=200) 
 ![](/images/screen3.png?width=200)    ![](/images/screen4.png?width=200) 
 ![](/images/screen5.png?width=200)    ![](/images/screen6.png?width=200) 
