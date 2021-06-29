# hello-world
Nothing much to say here, just testing

## Setting up FHIR resource dependancies (WHO COVID-19 Surveillance Package)
The following resources must be instantiated manually before submitting data.


### Organization resource

```sh
{
	"resourceType": "Organization",
	"id": "123456",
	"name": "KEMRI Clinic",
	"identifier": [
    {
      "system": "http://www.acme.org/practitioners",
      "value": "123456"
    }
  ]
}
```

### Practitioner resource

```sh
{
  "resourceType": "Practitioner",
  "id": "doc123",
  "text": {
    "status": "generated",
    "div": "<div xmlns=\"http://www.w3.org/1999/xhtml\">\n      <p>Dr Adam Careful is a Referring Practitioner for Acme Hospital from 1-Jan 2012 to 31-Mar\n        2012</p>\n    </div>"
  },
  "identifier": [
    {
      "system": "http://www.acme.org/practitioners",
      "value": "doc123"
    }
  ]
  
}
