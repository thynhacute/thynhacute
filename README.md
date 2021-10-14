### Nice to meet you ^^ I'm Thy (Hana) 👋

## I'm University Student ^^ ❤️
- 🥰 I wanna try everything I wanna try even though I could fail.
- 💎 Goals: To be a Great Tester.
- 🌸 My hobbies: studying, listening to music and traveling.

🥺❤️☘️🌸🌈🍒📷💎🎀

### Connect with me:


<a href="https://twitter.com/OrieHana"><img align="left" alt="OrieHana| Twitter" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/twitter.svg" /></a>
<a href="https://www.linkedin.com/in/thyy-nh%C3%A3-646867216//"><img align="left" alt="thyy-nh%C3%A3-646867216| LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" /></a>
<a href="https://www.instagram.com/__almira.hana/"><img align="left" alt="__almira.hana| Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" /></a>
<a href="https://www.facebook.com/OrieSocuteee/"><img align="left" alt="OrieSocuteee| Facebook" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/facebook.svg" /></a>
<br />
---
name: Latest YouTube Videos
on:
  schedule:
    # Runs every hour
    - cron: '0 * * * *'
  workflow_dispatch:

jobs:
  update-readme-with-youtube:
    name: Update this repo's README with latest videos from YouTube
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: gautamkrishnar/blog-post-workflow@master
        with:
          comment_tag_name: "YOUTUBE"
          feed_list: "https://www.youtube.com/feeds/videos.xml?channel_id=UCJey4xCkXQFBMmGQPtegtbw"

