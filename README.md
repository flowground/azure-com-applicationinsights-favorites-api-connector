# ![LOGO](logo.png) ApplicationInsightsManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ApplicationInsightsManagementClient API (version 2015-05-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/applicationinsights-favorites_API/2015-05-01/swagger.json<br/>
Generated at: 2019-06-11T18:13:19+03:00

## API Description

Azure Application Insights client for favorites.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets a list of favorites defined within an Application Insights component.

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `favoriteType` - _optional_ - The type of favorite. Value can be either shared or user.
    Possible values: shared, user.
* `sourceType` - _optional_ - Source type of favorite to return. When left out, the source type defaults to 'other' (not present in this enum).
    Possible values: retention, notebook, sessions, events, userflows, funnel, impact, segmentation.
* `canFetchContent` - _optional_ - Flag indicating whether or not to return the full content for each applicable favorite. If false, only return summary content for favorites.
* `tags` - _optional_ - Tags that must be present on each favorite returned.

### Remove a favorite that is associated to an Application Insights component.

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `favoriteId` - _required_ - The Id of a specific favorite defined in the Application Insights component

### Get a single favorite by its FavoriteId, defined within an Application Insights component.

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `favoriteId` - _required_ - The Id of a specific favorite defined in the Application Insights component

### Updates a favorite that has already been added to an Application Insights component.

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `favoriteId` - _required_ - The Id of a specific favorite defined in the Application Insights component

### Adds a new favorites to an Application Insights component.

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - The Azure subscription ID.
* `resourceName` - _required_ - The name of the Application Insights component resource.
* `favoriteId` - _required_ - The Id of a specific favorite defined in the Application Insights component

## License

**flow**ground :- Telekom iPaaS / azure-com-applicationinsights-favorites-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
