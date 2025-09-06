---
description: Simple Step-by-Step Guide
icon: telegram
---

# Telegram API Key Walkthrough

## Step 1: Create Your Telegram Bot

* Open Telegram and start a chat with **BotFather**.
* Type the command `/newbot` to create a new bot.
* Follow the prompts to:
  * Set a name for your bot.
  * Set a unique username (must end in `bot`).
* Once done, you’ll receive a **bot token** (e.g., `123456789:ABCdefGhIjKlmNoPQRstuVWXyz`).

More detailed tutorial here - [core.telegram.org/bots/tutorial](https://core.telegram.org/bots/tutorial)

Keep this token secure. You’ll use it later on aigent.run.

<figure><img src="../../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

## Step 2: Add Bot Token to aigent.run

* Visit [aigent.run](https://aigent.run) and go to the **Configuration** tab.
* Paste your **bot token** into the **Bot Token** field.
* Click **Save**.
* Use the **Test Credentials** button to check that the bot is connected correctly.

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

## Step 3: Add the Bot to a Telegram Group

* Create a new Telegram group or use one where you're already an admin.
* Add your newly created bot to the group.
* Once added, tap the group name → **Manage Group** → **Administrators**.
* Promote your bot to **Administrator** status.

<figure><img src="../../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

## Step 4: Get the Group Chat ID

To get the chat ID you have to follow these steps:

* Add @myidbot to the group you want to enable the agent in, and make it an Admin.
* Contact the [@myidbot](https://t.me/myidbot) bot and send the `/getid` command to get your personal chat ID, or invite it into a group and use the `/getgroupid` command to get the group chat ID.
* To get the Thread ID, the easiest way is this: Post a message to that topic, then right-click on it and select `Copy Message Link`. Paste it on a notepad and notice that it has the following structure `https://t.me/c/XXXXXXXXXX/YY/ZZ`. The Thread ID is `YY` (integer).

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

## Step 5: Add the Chat ID to aigent.run

1. Go back to the **Configuration** tab on aigent.run.
2. Paste the **Chat ID** into the appropriate field.
3. Click **Send Test Message**.

If everything is set up correctly, you’ll receive a message in your Telegram group saying:

"This is a test message from your AIgent."

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

That’s it! Your Telegram bot is now ready to send messages through aigent.run.
