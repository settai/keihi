[![Stories in Ready](https://badge.waffle.io/settai/uozumi.png?label=ready&title=Ready)](https://waffle.io/settai/uozumi)
# uozumi

## Getting Started (docker)

1. Install docker and docker-compose

2. Clone uozumi

        git clone https://github.com/settai/uozumi

3. Create database.yml

        cd uozumi
        cp config/database.yml{.sample,}

4. Create and start containers

        docker-compose up

5. Install gems

        docker_bin/bundle install

6. Boot servers

        docker_bin/rails s -b 0.0.0.0

7. Setup db

        docker_bin/rake db:setup

8. Access your site
  - for boot2docker user

    First, find out the IP address of your boot2docker host.

          boot2docker ip
          > 192.168.59.103

    Then you can access Uozumi to this url: http://192.168.59.103:8080

  - for others

    Access to http://localhost:8080
