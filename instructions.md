# How to setup SSL
1. Edit file `app.conf.example`
    1. Copy it to `data/nginx` as `app.conf`
    1. Change every ocurrence of `example.com` to your domain
1. Edit file `init-letsencrypt.sh.example`
    1. Save it as `init-letsencrypt.sh`
    1. Add permissions to execute this script `chmod +x init-letsencrypt.sh`
    1. Change every ocurrence of `example.org` to your domain
    1. Set your email in line 10
    
