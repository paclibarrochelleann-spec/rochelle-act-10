# Laboratory Activity 10 - AWS Lightsail deployment: Rochelle

Repo: `rochelle-act-10`. This is the Lab 9 app plus the `deploy/` folder.

Before AWS, set the partner in `app.py` (`PARTNER_URL`) to your partner's static IP, for example `http://PARTNER-STATIC-IP/api/students`, then push.

## Server (browser SSH on the Lightsail Ubuntu instance)
```
cd ~
git clone https://github.com/paclibarrochelleann-spec/rochelle-act-10.git
cd rochelle-act-10
bash deploy/setup_server.sh https://github.com/paclibarrochelleann-spec/rochelle-act-10.git
```
Then in Lightsail: Networking -> allow TCP 80 (not 8000) -> Create static IP -> attach.

## Update from GitHub
```
bash ~/rochelle-act-10/deploy/update_from_github.sh
```

## Troubleshooting
```
bash ~/rochelle-act-10/deploy/troubleshoot.sh
```

Use fictional data only. Never commit `.pem` keys or tokens. Stop or delete the instance and release the static IP when grading is done.
