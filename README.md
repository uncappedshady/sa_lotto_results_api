# South African Lottery Results API

## API Info

This API is currently in testing and is available for free with a quota of **100 API calls per day**.
You are allowed to generate an API key once per IP every 7 days.
In the current version, the API provides the latest lottery results for all South African game types including Daily Lotto, Lotto, Lotto Plus 1, Lotto Plus 2, Powerball, and Powerball Plus.
In the future paid version, there will be more API calls available, allowing you to retrieve lottery results per game type for specific dates.

## Notice

This API is currently in testing and is **free to use for now**. It provides the latest draw results for all South African lottery game types. In the future and in the paid version, users will be able to pull draw results for specific game types as well as for specific draw dates.

## Generate Your API Key

To access the latest lottery results through our API, you can generate an API key using the button on our [API page](https://resultsZA.co.za/generate_api_key).

## How to Use the API

Once you have your API key, you can make a request to our endpoint to retrieve the latest lottery results. Here's an example of how to make a request:

```http
GET https://resultsZA.co.za/api/get_latest_results?api_key=YOUR_API_KEY
```

Please replace `YOUR_API_KEY` with the key generated above.

### Response Format

The response will be a JSON object containing the latest draw results, structured as follows:

```json
{
    "status": "success",
    "results": [
        [
            "Draw Number",
            "Game Name",
            "Day of the Week",
            "Draw Date (GMT)",
            "Numbers (Array of drawn numbers)",
            "Bonus Number (if applicable)"
        ],
        
    ]
}
```

### Example response:

```json
{
    "status": "success",
    "results": [
        [1234,"Sample Game","Monday","Mon, 14 Aug 2000 00:00:00 GMT","[10, 20, 30, 40, 50]", "5"]
    ]
}
```

## Support and Feedback

We appreciate your feedback as we continue to test and improve this service. If you encounter any issues or have suggestions for enhancements, please leave your comments.

## License

This project is in development and may have certain limitations. Please refer to our [Terms and Conditions](https://resultsZA.co.za/privacy-policy) for more details.

## About Us

Visit our [website](https://resultsZA.co.za) to learn more about our services and other products.

## Disclaimer and Limitation of Liability

Please be advised that our website and this API project are independently operated and managed. We are in no way affiliated with, endorsed by, or sponsored by any lottery commission or governing body. This project's sole purpose is to capture and organize past draw results from publicly available sources, making it more convenient for users to retrieve this information via our API.

All information provided through this API, including draw results and other related data, is for informational purposes only. While we strive to maintain the accuracy and reliability of the information, we make no warranties or representations as to the correctness, accuracy, or reliability of any information provided. Users are encouraged to verify lottery results through official lottery channels.

By accessing or using this API, you agree to do so at your own risk, acknowledging that we shall not be liable for any inaccuracies, omissions, or errors in the information provided, or for any actions taken based on this information.

This API is intended for personal use and should not be utilized for commercial purposes without proper authorization and adherence to all applicable laws and regulations.

Your use of this API constitutes acceptance of these terms and any additional terms and conditions found on our [website](https://resultsZA.co.za/privacy-policy). We reserve the right to modify or update these terms at any time without prior notice.


