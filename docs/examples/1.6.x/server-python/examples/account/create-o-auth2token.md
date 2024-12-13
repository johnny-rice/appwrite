from appwrite.client import Client
from appwrite.enums import OAuthProvider

client = Client()
client.set_endpoint('https://cloud.appwrite.io/v1') # Your API Endpoint
client.set_project('<YOUR_PROJECT_ID>') # Your project ID

account = Account(client)

result = account.create_o_auth2_token(
    provider = OAuthProvider.AMAZON,
    success = 'https://example.com', # optional
    failure = 'https://example.com', # optional
    scopes = [] # optional
)