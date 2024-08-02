<div align="center">
<a href="https://curencee.pro"><img src="public/logo.png" alt="logo" width="40px"></a>  
</div>

<div align="center">
<h1>Currencee</h1>
<p>The World's Most Trusted, Fast and Secure Currency Converter</p> 
</div>

<img src="https://res.cloudinary.com/victoreke/image/upload/v1722546085/currencee/cover.png">

<br />
<div align="center">
<a href="https://www.producthunt.com/posts/currencee?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-currencee" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=351079&theme=light" alt="Currencee - Trusted | Product Hunt" style="width: 190px; height: 54px;" width="250" height="54" /></a>
</div><br>

[![Netlify Status](https://api.netlify.com/api/v1/badges/f7c5c576-f1b4-40f9-ba1b-6a39ec0ffa1d/deploy-status)](https://app.netlify.com/sites/currencee/deploys)

## Run project locally

- First generate your own API keys from [Currencybeacon](https://currencybeacon.com)
- Fork and clone the project to your machine.
- Rename `.env.example` to `.env`
- Set `API_KEY` to your own API credentials
- Set `PRODUCTION_URL` to your site's URL (Only relevant for production)
- Run the commands below

```sh
npm install
# First start the API server
npm run server

# Run development server on a separate terminal
npm run dev
```

Now you can visit [localhost:5173](http://localhost:5173) to see the project live.

## Server

This project utilizes an Express backend to hide the API credentials. To view the API in production, follow the steps below:

- If the API server is already running, skip to the next step, if not, run `npm run server` to start the API server
- Visit [localhost:8000/currency](http://localhost:8000/currency) to see the currency list
- Visit [localhost:8000/convert](http://localhost:8000/convert) to perform a conversion

> [!IMPORTANT]
> The convert endpoint takes in three parameters, a base currency code `base`, a foreign currency code `foreign`, and the `amount` you would like to convert.

Example endpoint

```
http://localhost:8000/convert?base=USD&foreign=NGN&amount=1
```

This should return an object that contains the conversion details.

> If you notice any bugs or errors, kindly raise an issue to discuss it. Contributions are also welcome.

## Attribution

The converter is powered by the [CurrencyBecacon API](https://currencybeacon.com), which supports over 161 commonly circulating world currencies listed [here](https://currencybeacon.com/supported-currencies). These cover 99% of all UN recognized states and territories.

The flags used are embedded using [Flagcdn](https://flagcdn.com/) which offers countries images based on their code.

<a href="https://www.buymeacoffee.com/victoreke">
  <img width="140px" alt="bmc-button" src="https://user-images.githubusercontent.com/62628408/127788747-8850d386-fc61-4fff-b18f-8c5ee597be34.png">
</a>
