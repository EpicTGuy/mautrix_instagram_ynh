## Log in to Instagram

1. In your Matrix client, start a direct chat with `@__BOTNAME__:__SERVER_NAME__` (if the account isn't found in the user directory, type the full ID).
2. Send `login instagram`. The bot asks for your instagram.com cookies, as a JSON object or as a cURL command.
3. In a desktop browser logged in to instagram.com, open the developer tools (`F12` or `Cmd+Option+I`) → **Network** tab, reload the page, right-click any request to `www.instagram.com` → **Copy** → **Copy as cURL**, and paste it as a reply to the bot.
4. Once logged in, your conversations appear as Matrix rooms. Delete the message containing the cookies from the chat with the bot, and **don't log out** of instagram.com in that browser (it would invalidate the session).

Useful commands (in the bot chat): `help`, `list-logins`, `logout <login ID>`.

If something doesn't work: `sudo yunohost service log __APP__` or `/var/log/__APP__/__APP__.log`.
