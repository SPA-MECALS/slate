# Login

## Login to an account

<blockquote class="lang-specific json">
  <p>The request returns a JSON structured like this (this is a pure exemple that is not working): </p>
</blockquote>

```json
{
  "worker_profiles": [
    {
      "worker_profile": {
        "id": 123456,
        "pub_id": "1234abcd",
        "active": true,
        "name": "Doe",
        "first_name": "John",
        "date_of_birth": null,
        "created_at": "2017-01-01T00:00:00.000Z",
        "updated_at": "2017-01-01T00:00:00.000Z",
        "facility_id": 123456,
        "user_id": 123456
      },
      "facility": {
        "id": 123456,
        "pub_id": "1234abcd",
        "active": true,
        "name": "Facility Name",
        "location": null,
        "created_at": "2017-01-01T00:00:00.000Z",
        "updated_at": "2017-01-01T00:00:00.000Z"
      }
    },
    {
      "worker_profile": {
        "id": 123456,
        "pub_id": "1234abcd",
        "active": true,
        "name": "Doe",
        "first_name": "John",
        "date_of_birth": null,
        "created_at": "2017-01-01T00:00:00.000Z",
        "updated_at": "2017-01-01T00:00:00.000Z",
        "facility_id": 123456,
        "user_id": 123456
      },
      "facility": {
        "id": 123456,
        "pub_id": "1234abcd",
        "active": true,
        "name": "Facility Name",
        "location": null,
        "created_at": "2017-01-01T00:00:00.000Z",
        "updated_at": "2017-01-01T00:00:00.000Z"
      }
    }
  ]
}
```

This endpoint allows you to login as an employe.

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
