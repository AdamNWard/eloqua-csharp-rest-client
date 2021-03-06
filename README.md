eloqua-csharp-rest-client
=========================

Eloqua C# Rest Client

## Usage

### Create Client
	var client = new Eloqua.Api.Rest.ClientLibrary.Client("site", "user", "pass");

### GET (item)
	int emailId = 1;	
	Email email = client.Assets.Email.Get(emailId);

### GET (list)
	List<Email> emails = client.Assets.Email.Get("searchTerm", pageNumber, pageSize);

### POST
	Email email = new Email() { ... };
	email = client.Assets.Email.Post(Email);

### PUT
	Email email = new Email() { ... };	
	email = client.Assets.Email.Put(Email);

### DELETE
	int emailId = 1;	
	client.Assets.Email.Delete(emailId);

## License
	Copyright [2012] [Fred Sakr]
	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at
	http://www.apache.org/licenses/LICENSE-2.0
	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.