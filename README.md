# ID.me Solution Consultant Exercise
This is Francisco Esqueda's exercise submission
Modeled after the provided sample seed Python Web App integrated with ID.me via OAuth 2.0

# Installation and Setup
Setup AWS EC2 - Amazon Linux instance

Install Prereqs
sudo pip install git
sudo pip install pip

Clone repo
git clone https://github.com/franciscoa19/id-me.git

Go to directory
cd id-me


Set your client configuration settings in `server.py`

````bash
# server.py
client_id              = 'YOUR_CLIENT_ID'
client_secret          = 'YOUR_CLIENT_SECRET'
redirect_uri           = 'YOUR_REDIRECT_URI'
authorization_base_url = 'https://api.id.me/oauth/authorize'
token_url              = 'https://api.id.me/oauth/token'
attributes_url         = 'https://api.id.me/api/public/v3/attributes.json'

# possible scope values: "military", "student", "responder", "government", "teacher"
scope = ['YOUR_SCOPE_VALUE']
````

Run the following to install the dependencies and start the server.

````bash
pip install -r requirements.txt
python server.py
````

Now you can view the app at fran.app
