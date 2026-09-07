For a repo in git hub create a webhook under settings:
https://github.com/arash-afk/Webhooks/settings/hooks

Using this listener provider:
https://webhook.site/

for decoding url like outcome from webhook.site
https://meyerweb.com/eric/tools/dencoder/

Redeliver as needed


## Following tests are also possible:
### Option 1: Use GitHub’s "Redeliver" Button (Fastest & Easiest)

GitHub saves every webhook payload sent over the last 3 days. You can instantly resend any past payload to `webhook.site` with a single click without pushing new code.

1.  Go to your GitHub repository.
    
2.  Click **Settings** (top toolbar) $\rightarrow$  **Webhooks** (left sidebar).
    
3.  Click on your `webhook.site` URL in the list.
    
4.  Click the **Recent Deliveries** tab.
    
5.  Click on any past delivery (the line with a green checkmark or red X) to expand it.
    
6.  Click the **Redeliver** button.
    

_Check your `webhook.site` tab—you will immediately see the exact same payload hit your dashboard again._

### Option 2: Trigger a New Event manually

If you want to test how GitHub handles real changes, trigger a new event on your repository:

-   **For Push events:** Make a small edit (e.g., add a comment to a `README.md` or text file directly in GitHub's web interface) and click **Commit changes**.
    
-   **For Issue events:** Go to the **Issues** tab in your repository and open or close a dummy issue.
    
-   **For Pull Requests:** Open a temporary branch, make a change, and open a Pull Request.
    

### Option 3: Send a "Ping" Payload

If you ever want to verify whether the connection between GitHub and `webhook.site` is still working:

1.  Go back to **Settings** $\rightarrow$ **Webhooks** $\rightarrow$ Click your webhook.
    
2.  Click **Edit** in the top right.
    
3.  Scroll down and click **Ping**. GitHub will immediately fire a lightweight test payload (`zen` text message) to your `webhook.site` URL.