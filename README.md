# Discord-bot-with-Rust
This bot implements the following features:

User Management:

The !kick command allows users with the appropriate permissions to kick mentioned users.


Game:

The !roll command generates a random number between 1 and 100, simulating a dice roll.


Automatic Moderation:

Basic spam protection: The bot tracks the time of the last message for each user and deletes messages if they're sent too quickly (less than 1 second apart).


Other Commands:

The !ping command responds with "Pong!" to check if the bot is responsive.



To use this bot:

Replace "YOUR_BOT_TOKEN_HERE" with your actual Discord bot token.
Make sure you have the necessary dependencies in your Cargo.toml:

[dependencies]
serenity = "0.11"
tokio = { version = "1.0", features = ["macros", "rt-multi-thread"] }
rand = "0.8"

Run the bot using cargo run.

This bot provides a foundation that you can expand upon. Here are some ideas for further development:

Implement more advanced games or interactive features.
Add more moderation commands (e.g., ban, mute).
Implement a warning system for users who break rules.
Create custom commands for server-specific needs.
Add logging functionality to track user actions and bot events.

Remember to handle errors appropriately and add more detailed permissions checks as needed for your specific use case.
