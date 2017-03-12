# Logout

## Logout of a workstation

<blockquote class="lang-specific json">
  <p>The request doesn't returns a JSON</p>
</blockquote>

```json

```

This endpoint allows you to logout of a workstation.

### HTTP Request

`POST http://193.10.30.169/logout`

### Query Parameters

The parameters to pass must be in the form of a JSON body.

Property | Type | Required | Description
-------- | ---- | -------- | -----------
user_id | string | true | Id of the user you want to logout
workstation_id | string | true | Id of the workstation where the user is login

### Return Codes

Code | Description
---- | -----------
200 | Success -- OK
401 | Unauthorized
