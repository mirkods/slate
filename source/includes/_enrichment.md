# Enrichment
The Enrichment API lets you look up person and company data based on an email or domain. For example, you could retrieve a person’s name, location and social handles from an email. Or you could lookup a company’s location, headcount or logo based on their domain name.

## Combined
A common use-case is looking up a person and company simultaneously based on a email address. To save you making two requests to do this, we offer a combined lookup API.

This endpoint expects an email address, and will return an object containing both the person and company (if found). A call to the combined lookup will only count as one API call.


```shell
curl "https://api.talentgarden.net/enrichment/v1/combined?email=davide.dattoli@talentgarden.org"
  -H "x-api-key: YOUR_API_KEY"
```

> The above command returns JSON structured like this:

```json
{
	"options": {},
	"person": {
		"id": "1d5d98b6-7703-425c-8087-d04ea335216d",
		"name": {
			"fullName": "Davide Dattoli",
			"givenName": "Davide",
			"familyName": "Dattoli"
		},
		"email": "davide.dattoli@talentgarden.org",
		"gender": null,
		"location": "IT",
		"timeZone": "Europe/Vatican",
		"utcOffset": 1,
		"geo": {
			"city": null,
			"state": null,
			"stateCode": null,
			"country": "Italy",
			"countryCode": "IT",
			"lat": 41.87194,
			"lng": 12.56738
		},
		"bio": "The best way to predict the future is to invent it. - President of @TalentGardenen Shaping a new way of Work, Learn and Connect",
		"site": "http://www.davidedattoli.it",
		"avatar": "https://d1ts43dypk8bqh.cloudfront.net/v1/avatars/1d5d98b6-7703-425c-8087-d04ea335216d",
		"employment": {
			"domain": "talentgarden.org",
			"name": "Talent Garden",
			"title": "CEO, Talent Garden, Talent Garden",
			"role": "ceo",
			"seniority": "executive"
		},
		"facebook": {
			"handle": "davidedattoli"
		},
		"github": {
			"handle": null,
			"id": null,
			"avatar": null,
			"company": null,
			"blog": null,
			"followers": null,
			"following": null
		},
		"twitter": {
			"handle": "davidedattoli",
			"id": 14523150,
			"bio": "The best way to predict the future is to invent it. - President of @TalentGardenen Shaping a new way of Work, Learn and Connect",
			"followers": 10609,
			"following": 1331,
			"statuses": 19904,
			"favorites": 4179,
			"location": "Brescia ✈ Milan ✈ New York",
			"site": "http://www.davidedattoli.it",
			"avatar": "https://pbs.twimg.com/profile_images/2539077588/1h7p22673pueqyq9ds9k.png"
		},
		"linkedin": {
			"handle": "in/davidedattoli"
		},
		"googleplus": {
			"handle": null
		},
		"aboutme": {
			"handle": null,
			"bio": null,
			"avatar": null
		},
		"gravatar": {
			"handle": null,
			"urls": null,
			"avatar": null,
			"avatars": []
		},
		"fuzzy": false,
		"emailProvider": false,
		"indexedAt": "2018-11-10T03:40:25.307Z"
	},
	"company": {
		"id": "6b0524b2-9c2d-4988-990e-afd5492f1673",
		"name": "Talent Garden",
		"legalName": null,
		"domain": "talentgarden.org",
		"domainAliases": [
			"talentgarden.ie",
			"talentgarden.es",
			"talentgarden.at",
			"talentgarden.co",
			"talentgarden.co.uk"
		],
		"site": {
			"phoneNumbers": [],
			"emailAddresses": [
				"info@talentgarden.org"
			]
		},
		"category": {
			"sector": "Information Technology",
			"industryGroup": "Software & Services",
			"industry": "Internet Software & Services",
			"subIndustry": "Internet",
			"sicCode": "87",
			"naicsCode": "54"
		},
		"tags": [
			"Marketplace",
			"B2B",
			"B2C",
			"Internet"
		],
		"description": "Talent Garden creates campuses to empower digital tech communities and connect them globally: coworking space, digital training, and networking. Join us!",
		"foundedYear": null,
		"location": "Via Cipro, 66, 25124 Brescia BS, Italy",
		"timeZone": "Europe/Rome",
		"utcOffset": 1,
		"geo": {
			"streetNumber": "66",
			"streetName": "Via Cipro",
			"subPremise": null,
			"city": "Brescia",
			"postalCode": "25124",
			"state": "Lombardia",
			"stateCode": null,
			"country": "Italy",
			"countryCode": "IT",
			"lat": 45.5246905,
			"lng": 10.2104083
		},
		"logo": "https://logo.clearbit.com/talentgarden.org",
		"facebook": {
			"handle": "talentgarden",
			"likes": 57056
		},
		"linkedin": {
			"handle": "company/talent-garden"
		},
		"twitter": {
			"handle": "talentgardenen",
			"id": "1291422799",
			"bio": "The place for explorers and innovators. #TalentGarden",
			"followers": 2459,
			"following": 726,
			"location": "",
			"site": "http://t.co/B91DTO9Gge",
			"avatar": "https://pbs.twimg.com/profile_images/882185915665448965/8K9la42a_normal.jpg"
		},
		"crunchbase": {
			"handle": "organization/talent-garden"
		},
		"emailProvider": false,
		"type": "private",
		"ticker": null,
		"identifiers": {
			"usEIN": null
		},
		"phone": null,
		"metrics": {
			"alexaUsRank": null,
			"alexaGlobalRank": null,
			"employees": 75,
			"employeesRange": "51-250",
			"marketCap": null,
			"raised": 12990000,
			"annualRevenue": null,
			"estimatedAnnualRevenue": "$10M-$50M",
			"fiscalYearEnd": null
		},
		"indexedAt": "2018-10-25T06:47:29.859Z",
		"tech": [
			"mailchimp",
			"google_apps",
			"activecampaign",
			"google_tag_manager",
			"facebook_advertiser",
			"facebook_connect",
			"nginx",
			"wordpress",
			"google_maps",
			"youtube",
			"sumo",
			"piwik",
			"google_analytics",
			"hubspot"
		],
		"parent": {
			"domain": null
		}
	}
}
```

This endpoint retrieves all informations about a company.

### HTTP Request

`GET https://api.talentgarden.net/enrichment/v1/combined?email=:email`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
email | true | the person’s email address

<aside class="notice">
This API is private. If you don't have an API KEY <a mailto="digital@talentgarden.org">get in touch with us</a>
</aside>


## Company
The Company API allows you to look up a company by their domain. Alongside the domain you may also provide any additional attributes you have about the company, such as their company name or twitter handle. Including more detail will help us be more accurate when searching.


```shell
curl "https://api.talentgarden.net/enrichment/v1/companies?domain=talentgarden.org"
  -H "x-api-key: YOUR_API_KEY"
```

> The above command returns JSON structured like this:

```json
{
	"id": "6b0524b2-9c2d-4988-990e-afd5492f1673",
	"name": "Talent Garden",
	"legalName": null,
	"domain": "talentgarden.org",
	"domainAliases": [
		"talentgarden.ie",
		"talentgarden.es",
		"talentgarden.at",
		"talentgarden.co",
		"talentgarden.co.uk"
	],
	"site": {
		"phoneNumbers": [],
		"emailAddresses": [
			"info@talentgarden.org"
		]
	},
	"category": {
		"sector": "Information Technology",
		"industryGroup": "Software & Services",
		"industry": "Internet Software & Services",
		"subIndustry": "Internet",
		"sicCode": "87",
		"naicsCode": "54"
	},
	"tags": [
		"Marketplace",
		"B2B",
		"B2C",
		"Internet"
	],
	"description": "Talent Garden creates campuses to empower digital tech communities and connect them globally: coworking space, digital training, and networking. Join us!",
	"foundedYear": null,
	"location": "Via Cipro, 66, 25124 Brescia BS, Italy",
	"timeZone": "Europe/Rome",
	"utcOffset": 1,
	"geo": {
		"streetNumber": "66",
		"streetName": "Via Cipro",
		"subPremise": null,
		"city": "Brescia",
		"postalCode": "25124",
		"state": "Lombardia",
		"stateCode": null,
		"country": "Italy",
		"countryCode": "IT",
		"lat": 45.5246905,
		"lng": 10.2104083
	},
	"logo": "https://logo.clearbit.com/talentgarden.org",
	"facebook": {
		"handle": "talentgarden",
		"likes": 57056
	},
	"linkedin": {
		"handle": "company/talent-garden"
	},
	"twitter": {
		"handle": "talentgardenen",
		"id": "1291422799",
		"bio": "The place for explorers and innovators. #TalentGarden",
		"followers": 2459,
		"following": 726,
		"location": "",
		"site": "http://t.co/B91DTO9Gge",
		"avatar": "https://pbs.twimg.com/profile_images/882185915665448965/8K9la42a_normal.jpg"
	},
	"crunchbase": {
		"handle": "organization/talent-garden"
	},
	"emailProvider": false,
	"type": "private",
	"ticker": null,
	"identifiers": {
		"usEIN": null
	},
	"phone": null,
	"metrics": {
		"alexaUsRank": null,
		"alexaGlobalRank": null,
		"employees": 75,
		"employeesRange": "51-250",
		"marketCap": null,
		"raised": 12990000,
		"annualRevenue": null,
		"estimatedAnnualRevenue": "$10M-$50M",
		"fiscalYearEnd": null
	},
	"indexedAt": "2018-10-25T06:47:29.859Z",
	"tech": [
		"mailchimp",
		"google_apps",
		"activecampaign",
		"google_tag_manager",
		"facebook_advertiser",
		"facebook_connect",
		"nginx",
		"wordpress",
		"google_maps",
		"youtube",
		"sumo",
		"piwik",
		"google_analytics",
		"hubspot"
	],
	"parent": {
		"domain": null
	}
}
```

This endpoint retrieves all informations about a company.

### HTTP Request

`GET https://api.talentgarden.net/enrichment/v1/companies?domain=:domain`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
domain | true | the company’s domain

<aside class="notice">
This API is private. If you don't have an API KEY <a mailto="digital@talentgarden.org">get in touch with us</a>
</aside>

## Person
The People API lets you retrieve social information associated with an email address, such as a person’s name, location and Twitter handle.

```shell
curl "https://api.talentgarden.net/enrichment/v1/people?email=alex@alexmaccaw.com"
  -H "Authorization: YOUR_API_KEY"
```

> The above command returns JSON structured like this:

```json
{
  "id": "d54c54ad-40be-4305-8a34-0ab44710b90d",
  "name": {
    "fullName": "Alex MacCaw",
    "givenName": "Alex",
    "familyName": "MacCaw"
  },
  "email": "alex@alexmaccaw.com",
  "location": "San Francisco, CA, US",
  "timeZone": "America/Los_Angeles",
  "utcOffset": -8,
  "geo": {
    "city": "San Francisco",
    "state": "California",
    "stateCode": "CA",
    "country": "United States",
    "countryCode": "US",
    "lat": 37.7749295,
    "lng": -122.4194155
  },
  "bio": "O'Reilly author, software engineer & traveller. Founder of https://clearbit.com",
  "site": "http://alexmaccaw.com",
  "avatar": "https://d1ts43dypk8bqh.cloudfront.net/v1/avatars/d54c54ad-40be-4305-8a34-0ab44710b90d",
  "employment": {
    "domain": "clearbit.com",
    "name": "Clearbit",
    "title": "Founder and CEO",
    "role": "ceo",
    "seniority": "executive"
  },
  "facebook": {
    "handle": "amaccaw"
  },
  "github": {
    "handle": "maccman",
    "avatar": "https://avatars.githubusercontent.com/u/2142?v=2",
    "company": "Clearbit",
    "blog": "http://alexmaccaw.com",
    "followers": 2932,
    "following": 94
  },
  "twitter": {
    "handle": "maccaw",
    "id": "2006261",
    "bio": "O'Reilly author, software engineer & traveller. Founder of https://clearbit.com",
    "followers": 15248,
    "following": 1711,
    "location": "San Francisco",
    "site": "http://alexmaccaw.com",
    "avatar": "https://pbs.twimg.com/profile_images/1826201101/297606_10150904890650705_570400704_21211347_1883468370_n.jpeg"
  },
  "linkedin": {
    "handle": "pub/alex-maccaw/78/929/ab5"
  },
  "googleplus": {
    "handle": null
  },
  "gravatar": {
    "handle": "maccman",
    "urls": [
      {
        "value": "http://alexmaccaw.com",
        "title": "Personal Website"
      }
    ],
    "avatar": "http://2.gravatar.com/avatar/994909da96d3afaf4daaf54973914b64",
    "avatars": [
      {
        "url": "http://2.gravatar.com/avatar/994909da96d3afaf4daaf54973914b64",
        "type": "thumbnail"
      }
    ]
  },
  "fuzzy": false,
  "emailProvider": false,
  "indexedAt": "2016-11-07T00:00:00.000Z"
}
```

This endpoint retrieves all informations about a person.

### HTTP Request

`GET https://api.talentgarden.net/enrichment/v1/people?email=:email`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
email | true | the person’s email address

<aside class="notice">
This API is private. If you don't have an API KEY <a mailto="digital@talentgarden.org">get in touch with us</a>
</aside>
