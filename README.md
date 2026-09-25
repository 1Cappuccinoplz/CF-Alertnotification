This test showcase how CF integrate with telegram bot to push notification when origin server or application have problem
or during maintance. 

The component use in this testcase: 
1. Cloudflare Health Check: Use to check if origin server or application is healthy or not.
2. Cloudflare Alert: Use to create alert notification sent to telegram bot.
3. Cloudflare Webhook: Use to integrate telegram bot API with Cloudflare to receive a message. 
4. Cloudflare Worker: As telegram bot API see a message in a different format from Cloudflare Webhook, worker act as
translator translate message from webhook to a format that telegram bot API understand.
5. Bot-daddy: Use to create telegram bot
   
