# Virtual-TryOn-Pro API Integration Guide

Advanced AI Virtual Try-On API for clothes, jewelry, and fashion items. Fits garments on any model perfectly in seconds.

## 🚀 Get Started
To get your API key and subscribe to a plan, visit our RapidAPI page:
👉 **[Virtual-TryOn-Pro on RapidAPI](https://rapidapi.com/)**

## 📦 Installation
Choose your preferred language to make the API call.

### Node.js (Axios)
```javascript
const axios = require('axios');

const options = {
  method: 'POST',
  url: '[https://virtual-tryon-pro.p.rapidapi.com/tryon](https://virtual-tryon-pro.p.rapidapi.com/tryon)',
  headers: {
    'content-type': 'application/json',
    'X-RapidAPI-Key': 'YOUR_RAPIDAPI_KEY',
    'X-RapidAPI-Host': 'virtual-tryon-pro.p.rapidapi.com'
  },
  data: {
    image: '[https://example.com/your-model-image.jpg](https://example.com/your-model-image.jpg)',
    prompt: 'A luxury black button-down dress shirt'
  }
};

async function run() {
  try {
    const response = await axios.request(options);
    console.log(response.data);
  } catch (error) {
    console.error(error);
  }
}

run();
<?php

$curl = curl_init();

curl_setopt_array($curl, [
  CURLOPT_URL => "[https://virtual-tryon-pro.p.rapidapi.com/tryon](https://virtual-tryon-pro.p.rapidapi.com/tryon)",
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => "",
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 30,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => "POST",
  CURLOPT_POSTFIELDS => json_encode([
    'image' => '[https://example.com/your-model-image.jpg](https://example.com/your-model-image.jpg)',
    'prompt' => 'A luxury black button-down dress shirt'
  ]),
  CURLOPT_HTTPHEADER => [
    "X-RapidAPI-Host: virtual-tryon-pro.p.rapidapi.com",
    "X-RapidAPI-Key: YOUR_RAPIDAPI_KEY",
    "content-type: application/json"
  ],
]);

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
  echo "cURL Error #:". $err;
} else {
  echo $response;
}
{
  "status": "success",
  "result_b64": "iVBORw0KGgoAAAANSUhEUgAA..."
}
