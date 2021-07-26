# Reisler All Bot (ReislerAllBot)

> A Telegram Bot implemented fetch all users automatically in the group and replace the keywords like `@all` to tag all users like `@sheiun @tom ...`.

## What problem we solved?

> Since there is no telegram api for fetching all users there is only `chat.get_administrators` and it cannot achieve our aim, tagging all users, so we propose a method to use `telethon` to login as a user and get all users' id via `GetParticipantsRequest` and retreive correspond user via `chat.get_member(user_id)`.

## Step to build your own `Metion All Memebers Bot`

> Or you can use our bot [Metion All Members Bot](https://t.me/MentionAllMembersBot)

1. Register a bot via [Bot Father](https://t.me/botfather)
2. Add the bot into your group and give it 'Invite users via link' and 'Delete messages' permissions
3. Register api key from <https://my.telegram.org/auth>
4. Edit your `config.json` like [config.example.json](config.example.json) to fill bot token, api id and api hash
5. Run `python dump_users.py` to dump users in a group via invite link
6. Run `python bot.py`

###  💜 Herokuya Dağıt

[![ Dağıt ](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/ReislerSupport/Etiketlemeci)
String üçün botdan kullanımdə edin [ @ReislerAllBot ](https://t.me/@ReislerAllBot)

###  ⚔ Sunucubağlama
```ş
# Git Yüklə (apt-instll git)
$ git klonu https://github.com/pischule/mention-all-bot.git aaa.      

{
  "token": "1759980514:AAHX8hBgI3MMShWoURc3cRTysmQ9Z2hvINQ",
  "api_id": 6113281,
  "api_hash": "0c46b31e35749f9f4006a7cadb3ed877",
  "links": ["invited_link_for_prefetching_group_members"],
  "keywords": ["@all", "@everyone", "@ReislerAllBot"]
}
{
  " name " : " Telgraf Yükleme Botu " ,
  " açıklama " : " telegra.ph bağlantı yükleyici botuna giden basit bir küçük ortam veya dosya " ,
  " depo " : " https://github.com/FayasNoushad/Telegraph-Uploader-Bot " ,
  " anahtar kelimeler " : [ " telgraf " , " dosya veya medya " , " bağlantı yükleyici " , " telgraf botu " ],
  " env " : {
    " BOT_TOKEN " : {
      " description " : " @Botfather'dan Bot jetonunuz "
    },
    " API_ID " : {
      " description " : " https://my.telegram.org/apps adresinden API_ID'niz "
    },
    " API_HASH " : {
      " description " : " https://my.telegram.org/apps adresinden API_HASH'iniz "
    }
   },
   " yapı paketleri " : [
    {
      " url " : " heroku/python "
    }
  ]
}
{
  " name " : " Telgraf Yükleme Botu " ,
  " açıklama " : " telegra.ph bağlantı yükleyici botuna giden basit bir küçük ortam veya dosya " ,
  " depo " : " https://github.com/FayasNoushad/Telegraph-Uploader-Bot " ,
  " anahtar kelimeler " : [ " telgraf " , " dosya veya medya " , " bağlantı yükleyici " , " telgraf botu " ],
  " env " : {
    " BOT_TOKEN " : {
      " description " : " @Botfather'dan Bot jetonunuz "
    },
    " API_ID " : {
      " description " : " https://my.telegram.org/apps adresinden API_ID'niz "
    },
    " API_HASH " : {
      " description " : " https://my.telegram.org/apps adresinden API_HASH'iniz "
    }
   },
   " yapı paketleri " : [
    {
      " url " : " heroku/python "
    }
  ]
}
