Scopes for Optra are going to be in the following format
`resource_name:action:resource_name`
So for example`api:read_api:api_123`allows the client to read from only api_123.
To read all apis the client would need`api:read_api:*`.
Need to have the following permission for Optra API.
- [ ] `api:read_api:*`Able to get/list all apis in the workspace.
- [ ] `api:read_api:<api_id>`Able to get/list only api_id.
- [ ] `api:create_api:*`Able to create apis.
- [ ] `api:update_api:*`Able to update all apis in the workspace. This includes adding and removing scopes.
- [ ] `api:update_api:<api_id>`. Able to update only api api_id. This includes adding and removing scopes.
- [ ] `api:delete_api:*`Able to delete all apis in the workspace.
- [ ] `api:delete_api:<api_id>`. Able to delete all apis.
- [ ] `api:create_client:*`Able to create clients for all apis in the workspace.
- [ ] `api:create_client:<api_id>`Able to create clients for only api api_id.
- [ ] `api:read_client:*`Able to read all clients for all apis in the workspace.
- [ ] `api:read_client:<api_id>`Able read clients for only api api_id.
- [ ] `api:update_client:*`Able to update clients for all apis in the workspace. This includes adding and removing scopes.
- [ ] `api:update_client:<api_id>`Able to update clients for only api api_id.
- [ ] `api:delete_client:*`Able to delete clients for all apis in the workspace.
- [ ] `api:delete_client:<api_id>`Able to delete clients for only api api_id.