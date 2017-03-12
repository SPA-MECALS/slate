# Logout

## Login to an account

```shell
curl -H "X-Key: YOUR XKEY" "https://backoffice.mailperformance.com/actions/"
```

<blockquote class="lang-specific json">
  <p>The request returns a JSON structured like this (this is a pure exemple that is not working): </p>
</blockquote>

```json

```

This endpoint retrieves all actions.

### HTTP Request

`POST http://193.10.30.169/login`

### Query Parameters

The parameters to pass must be in the form of a JSON body.

Property | Type | Required | Description
-------- | ---- | -------- | -----------
email | string | true | Email of the user you want to login with
password | string | true | Password of the user you want to login with


### Return Codes

Code | Description
---- | -----------
200 | Success -- OK
401 | Unauthorized -- Your credentials are wrong
