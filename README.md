# GWA Notification Receipt

> An [Azure Function app](https://azure.microsoft.com/en-gb/services/functions/)
> for receiving callbacks from
> [GOV.UK Notify](https://www.notifications.service.gov.uk/)

The app exposes an HTTP endpoint where Notify can POST a callback to. The
message is checked for correct authorization, added to a queue for processing
before updating a collection is Cosmos DB.

## Functions

The app is made up of a number of functions, each function is explained in more
detail in its' own README:

* [MessageReceiptHttpTrigger](MessageReceiptHttpTrigger/README.md)
* [MessageReceiptQueueTrigger](MessageReceiptQueueTrigger/README.md)

## License

THIS INFORMATION IS LICENSED UNDER THE CONDITIONS OF THE OPEN GOVERNMENT
LICENCE found at:

<http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3>

The following attribution statement MUST be cited in your products and
applications when using this information.

> Contains public sector information licensed under the Open Government license
> v3

### About the license

The Open Government Licence (OGL) was developed by the Controller of Her
Majesty's Stationery Office (HMSO) to enable information providers in the
public sector to license the use and re-use of their information under a common
open licence.

It is designed to encourage use and re-use of information freely and flexibly,
with only a few conditions.
