# How to set up SSL
1. Edit file `app.conf.example`
    1. Copy it to `data/nginx` as `app.conf`
    2. Change every occurrence of `example.com` to your domain
2. Edit file `init-letsencrypt.sh.example`
    1. Save it as `init-letsencrypt.sh`
    2. Add permissions to execute this script `chmod +x init-letsencrypt.sh`
    3. Change every occurrence of `example.org` to your domain
    4. Set your email in line 10
3. Run `sudo ./init-letsencrypt.sh`
4. Change ownership of data directory: `sudo chown ec2-user:ec2-user -R ./data`
5. Run `docker compose up -d`
