<script>
    let github_logo = "/github_logo.jpg"
    let links = [
        {
            "platform":"Github",
            "link": "https://github.com/h4ck0rman",
            "logo":"/github_logo.png",
            "logo_alt":"Github link logo"
        },
        {
            "platform":"LinkedIn",
            "link": "https://au.linkedin.com/in/puneeth-kambhampati-152909136",
            "logo":"/linkedin_logo.png",
            "logo_alt":"LinkedIn link logo"
        },
        {
            "platform":"TikTok",
            "link": "https://www.tiktok.com/@h4ck0rmanttv",
            "logo":"/tiktok_logo.png",
            "logo_alt":"TikTok link logo"
        },
        {
            "platform":"Twitch",
            "link": "https://www.twitch.tv/h4ck0rman",
            "logo":"/twitch_logo.png",
            "logo_alt":"Twitch link logo"
        },
    ]
</script>

<div class='container rounded-md hover:bg-slate-400 fixed riig'>
    <ul>
        {#each links as link}
        <div class="rounded h-7 w-7 bg-transparent hover:bg-orange-500">
            <li >
                <a href={link.link} target="_blank">
                    <img src={link.logo} alt={link.logo_alt}/>      
                </a>
            </li>
        </div>
        {/each}
    </ul>
    
</div>