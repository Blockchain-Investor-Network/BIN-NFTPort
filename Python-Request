import http.client

conn = http.client.HTTPSConnection("api.nftport.xyz")

payload = "{\n  \"chain\": \"polygon\",\n  \"contract_address\": \"0xC8D297D7b496f86673551c933815B47973FC4a0e\",\n  \"metadata_uri\": \"",\n  \"mint_to_address\": \"BSI_Address"\n}"

headers = {
    'Content-Type': "application/json",
    'Authorization': ""
    }

conn.request("POST", "/v0/mints/customizable", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
