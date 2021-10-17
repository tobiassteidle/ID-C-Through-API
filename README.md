# Identity Card and Passport classification API
Identify and classify IDs and passports on documents.

#### Endpoints
The Identity Card and Passport classification API is available on [RapidAPI](https://rapidapi.com/tssd/api/identity-card-and-passport-classification/).

URL (authentication required):  
https://identity-card-and-passport-classification.p.rapidapi.com/api/v1/identification


#### Supported ID Cards:
| COUNTRY 	| TYPE     	| FRONT 	            | EXAMPLE 	                                                            | BACK                 	| EXAMPLE                                                        	    |
|---------	|----------	|:-----:	            |----------	                                                            |------	                |----------	                                                            |
| Austria	| IDCARD 	| :heavy_check_mark:   	| ![austria_idcard_front](docs/assets/austria_idcard_front.jpg)   	    | :x:                  	|                                                               	    |
| Chile 	| IDCARD 	| :heavy_check_mark:   	| ![chile_idcard_front](docs/assets/chile_idcard_front.jpg)   	        | :x:                  	|                                                               	    |
| Czech 	| IDCARD 	| :heavy_check_mark:   	| ![czech_idcard_front](docs/assets/czech_idcard_front.jpg)   	        | :x:                  	|                                                               	    |
| Czech 	| PASSPORT 	| :heavy_check_mark:   	| ![czech_passport_front](docs/assets/czech_passport_front.jpg)         | :x:                  	|                                                               	    |
| Germany 	| IDCARD 	| :heavy_check_mark:   	| ![german_idcard_front](docs/assets/german_idcard_front.jpg)           | :heavy_check_mark:   	| ![german_idcard_back](docs/assets/german_idcard_back.jpg)      	    |
| Germany 	| IDCARD (old) 	| :heavy_check_mark:   	| ![german_idcard_old_front](docs/assets/german_idcard_old_front.jpg)   | :heavy_check_mark:   	| ![german_idcard_old_back](docs/assets/german_idcard_old_back.jpg)     |
| Germany 	| IDCARD (temporal) 	| :heavy_check_mark:   	| ![german_idcard_temporal_front](docs/assets/german_idcard_temporal_front.jpg)   | :heavy_check_mark:   	| ![german_idcard_temporal_back](docs/assets/german_idcard_temporal_back.jpg)     |
| Germany 	| PASSPORT 	| :heavy_check_mark:   	| ![german_passport_front](docs/assets/german_passport_front.jpg)       | :x:               	|                                                                       |
| Germany 	| RESIDENCE_PERMIT 	| :heavy_check_mark:   	| ![german_residencepermit_front](docs/assets/german_residencepermit_front.jpg)           | :heavy_check_mark:   	| ![german_residencepermit_back](docs/assets/german_residencepermit_back.jpg)      	    |

See [REST API Documentation](docs/REST_API.md) for sample request.

**Current Version:** [v2_20211014](docs/RELEASE_NOTES.md)

### Feature Request or request for new id cards
For additional features or support for more ID cards / passports etc. [please create an issue](https://github.com/tobiassteidle/Identity-Card-And-Passport-Classification-API/issues/new).

