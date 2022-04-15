# BT4222 Grp20 FakeNewsDetection Code Submission
Investigating and Detecting Fake News Spread on Social Media
# Data Collection 
Follow steps on 
1. Pull code from <https://github.com/KaiDMML/FakeNewsNet>
2. Follow the Installation guide and install all requirements from the github repo 
```
pip install -r requirements.txt
```
3. Edit the `code/config.json` file
4. Change `data_features_to_collect` to retrieve features for our dataset
5. Set up the a flask application to start collecting data.
```
nohup python -m resource_server.app &> keys_server.out&
```
6. Run the code 
```
nohup python main.py &> data_collection.out&
```
7. Store data in JSON file `politfact.json` and `gossipcop.json` for new article and `politfact_tweets.json` and `gossipcop_tweets.json` for tweets.    
