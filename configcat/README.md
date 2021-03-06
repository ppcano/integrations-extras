# ConfigCat

## Overview

Ensures that every setting change in ConfigCat is sent to DataDog as an Event.

![DataDogEvent][3]

## Setup

1. Have a [DataDog subscription][8].
2. Get a [DataDog API Key][9].
    ![DataDogEvent][1] 
4. Open the [integrations tab][10] on ConfigCat Dashboard.
5. Click on DataDog's _CONNECT_ button and set your DataDog API key.
6. You're all set. Go ahead and make some changes on your feature flags then check your Events in DataDog.


### Un-installation

1. Open the [integrations tab][10] on ConfigCat Dashboard.
2. Click on DataDog's DISCONNECT button and set your DataDog API key.

## Data Collected

### Metrics

ConfigCat integration does not include any metrics.

### Events

All ConfigCat related events collected appear within the DataDog Event Stream with the `source:configcat` property are tagged with your product, config and environment names.

For example here is how to search for events that happened in the production environment: `sources:configcat production`:

![Filtering][4]

### Service Checks

ConfigCat integration does not include any service checks.

## Troubleshooting

Need help? See the [ConfigCat documentation][6] or contact [ConfigCat support][7]

[1]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/configcat/images/datadog_apikey.png
[3]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/configcat/images/datadog_event.png
[4]: https://raw.githubusercontent.com/DataDog/integrations-extras/master/configcat/images/datadog_filtering.png
[6]: https://configcat.com/docs/integrations/datadog/
[7]: https://configcat.com/support
[8]: https://www.datadoghq.com
[9]: https://docs.datadoghq.com/account_management/api-app-keys/#api-keys
[10]: https://app.configcat.com/product/integrations
