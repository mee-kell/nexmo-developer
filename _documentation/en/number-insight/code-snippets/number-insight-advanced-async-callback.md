---
title: Number Insight Advanced Webhook
navigation_weight: 5
---

# Number Insight Advanced Webhook

This code snippet shows you how to code the webhook handler that receives the data returned by an asynchronous call to the Number Insight Advanced API. See the [Number Insight Advanced](/number-insight/code-snippets/number-insight-advanced-async) code snippet to learn how to code the initial request for the insight data.

Before attempting to run the code examples, replace the variable placeholders as instructed in [replaceable variables](/number-insight/code-snippets/before-you-begin#replaceable-variables).

```code_snippets
source: '_examples/number-insight/async-callback'
```

The response from the API contains the following data:

```json
{
    "status": 0,
    "status_message": "Success",
    "lookup_outcome": 0,
    "lookup_outcome_message": "Success",
    "request_id": "75fa272e-4743-43f1-995e-a684901222d6",
    "international_format_number": "447700900000",
    "national_format_number": "07700 900000",
    "country_code": "GB",
    "country_code_iso3": "GBR",
    "country_name": "United Kingdom",
    "country_prefix": "44",
    "request_price": "0.03000000",
    "remaining_balance": "10.000000",
    "current_carrier": {
        "network_code": "23420",
        "name": "Hutchison 3G Ltd",
        "country": "GB",
        "network_type": "mobile"
    },
    "original_carrier": {
        "network_code": "23410",
        "name": "Telefonica UK Limited",
        "country": "GB",
        "network_type": "mobile"
    },
    "valid_number": "valid",
    "reachable": "reachable",
    "ported": "ported",
    "roaming": {"status": "not_roaming"}
}
```

For a description of each returned field and to see all possible values, see the [Number Insights API documentation](/api/number-insight#asyncCallback)

