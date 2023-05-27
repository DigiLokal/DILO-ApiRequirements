# Api Requirements
The API requirements for DILO project.

Some samples will be given later.

Everything here is still temporary, changes are expected.

---



## User Registration:

- URL

  - `/register`

- Method

  - `POST`

- Parameters

  - `name` as string
  - `email` as string
  - `password` as string
  - `path` as string


## User Login:

- URL

  - `/login`

- Method

  - `POST`

- Parameters

  - `email` as string
  - `password` as string



## UMKM Home Page:

- URL

  - `/umkm/home`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <accessToken>`, optional




## Get All Services (Campaign)

- URL
  - `/umkm/services`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <accessToken>`, optional

- Parameters

  - `query` as string

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/get-all-services.json)


## Search Services (Campaign)

- URL
  - `/umkm/services/search`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <accessToken>`, optional

- Parameters

  - `query` as string

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/get-search-umkm.json)


## Detail Services (Campaign)

- URL
  - `/umkm/services/{serviceId}`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <accessToken>`

- Parameters

  - `campaignId` as string

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/get-services-details.json)



## Get Cart (Projects)

- URL
  - `/cart`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <accessToken>`

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/get-cart.json)


## Add to Cart (Projects)

- URL
  - `/cart/add`

- Method

  - `POST`

- Headers

  - Authorization: `Bearer <accessToken>`

- Parameters

  - `service_id` as string,

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/post-cart-add)



## Remove from Cart (Projects)

- URL
  - `/cart/remove`

- Method

  - `POST`

- Headers

  - Authorization: `Bearer <accessToken>`

- Parameters

  - `service_id` as string,

- Response
  - [Sample](https://github.com/DigiLokal/DILO-ApiRequirements/blob/main/response/post-cart-remove)

# UMKM/SME Path

# Digital Freelance Path

# Influencer Path
