# Api Requirements
The API requirements for DILO project (not done).

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

# The 'Full' List

- User Management APIs:

  - Profile APIs:
  - Get user profile: GET /profile
  - Update user profile: PUT /profile

- UMKM Path APIs:
  - Get UMKM home page content: GET /umkm/home
  - Search services: GET /umkm/services/search
  - Get detailed service information: GET /umkm/services/<service_id>

  - Post Campaign API:
  - Post Campaign (UMKM): POST /umkm/campaigns
  - Post Services (Freelance/Influencer): POST /umkm/campaigns

- Influencer APIs:
  - Get influencer list: GET /influencers
  - Get detailed influencer information: GET /influencers/<influencer_id>
  - Get influencer rate cards: GET /influencers/<influencer_id>/rate-cards
  - ?Get influencer reviews: GET /influencers/<influencer_id>/reviews

- Freelancer APIs:
  - Get freelancer list: GET /freelancers
  - Get detailed freelancer information: GET /freelancers/<freelancer_id>
  - Get freelancer rate cards: GET /freelancers/<freelancer_id>/rate-cards
  - ?Get freelancer reviews: GET /freelancers/<freelancer_id>/reviews

- Order Management APIs:
  - Add service to cart: POST /cart/add
  - Get cart items: GET /cart
  - Remove item from cart: DELETE /cart/remove
  - Checkout: POST /umkm/checkout
  - Get order details: GET /orders/<order_id>

- Chat APIs (?):
  - ?Send message: POST /chats/<recipient_id>/messages
  - ?Get messages: GET /chats/<recipient_id>/messages
  - ?Mark message as read: PUT /chats/<recipient_id>/messages/<message_id>/read

- Payment APIs:
  -

