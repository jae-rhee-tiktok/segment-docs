---
title: TikTok Offline Conversions Destination
id: 6447ca8bfaa773a2ba0777a0
hidden: true
---

{% include content/plan-grid.md name="actions" %}

[TikTok's Offline Events API](https://ads.tiktok.com/marketing_api/docs?id=1758049779688450){:target="_blank"} helps advertisers measure how TikTok ads result in offline customer actions, such as in-store purchases or offline subscriptions or purchases. Attributing online and offline events is an important step for advertisers to measure omni-channel results from their campaigns. 

## Benefits of TikTok Offline Conversions
- **Measure how TikTok ads influence offline conversions.** Learn what online strategies lead to better Brick & Mortar sales, subscription sign-ups or leads. 
- **Power holistic attribution models with cross-channel event tracking.** Combine online and offline touch points to get comprehensive campaign metrics, like ROAS.
- **Reach offline customers online with custom audiences.** Promote new products or services to high-value customers who initiative offline events.


This destination is maintained by TikTok. For any issues with the destination, [contact their Support team](mailto:segmenteng@bytedance.com).

{% include content/ajs-upgrade.md %}

## Getting started

Before you configure the TikTok Offline Conversions destination, create an Offline Event Set and generate the Access Token for it from the **TikTok Events Manager**. For more information, see TikTok's article, [Get Started](https://ads.tiktok.com/marketing_api/docs?id=1758051319816193){:target="_blank"}

To add and configure the TikTok Offline Conversions destination:

1. From the Segment web app, click **Catalog**, then click **Destinations**.
2. Find the Destinations Actions item in the left navigation, and click it.
3. Click **Configure Tiktok Offline Conversions (Actions)**.
4. Select an existing Source to connect to destination.
5. Give the Destination a name.
6. On the Settings screen, enter the  **Access Token** and **Event Set ID**.
7. Toggle on the Destination.
8. Click Save Changes.

{% include components/actions-fields.html %}

## PII Requirement & Validation
The TikTok Offline Events API requires that you include at least one type of PII (for example, email address or phone number) in all offline conversion events. Segment hashes these values with SHA-256 before it sends them to TikTok, so you do not need to hash them before they're ingested by Segment. In addition, the TikTok Offline Conversions Destination validates all offline events before it forwards them to the TikTok Offline Events API. The TikTok Offline Conversions Destination doesn't send any offline events to TikTok with invalid or missing PII.

## Data and Privacy Considerations
- Every offline event sent to the TikTok Offline Events API requires at least one email address or phone number.
- E-mails and phone numbers are hashed in a privacy-safe way by default so that TikTok cannot identify customers who are not TikTok users.
- iOS compliance checks are performed on PII (ATT opt-out users will still be reported and attributed).
- TikTok purges unmatched offline conversions IDs/records.

