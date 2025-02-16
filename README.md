## 🎯 Objective

- To create and play more with `strapi` + `gatsby`.

- This project was created following [this link here](https://www.gatsbyjs.com/blog/2018-1-18-strapi-and-gatsby/#1-introduction).

## 🔗 Link 

The CMS is available under the below link

https://strapi-with-gatsby-cms.herokuapp.com/admin/

## 🚀 Heroku / Deploying

![Heroku](https://heroku-badge.herokuapp.com/?app=strapi-with-gatsby-cms)

- `heroku create strapi-with-gatsby-cms`

- `heroku addons:create heroku-postgresql:hobby-dev`

- `heroku config`

```shell
postgres://liaxabdytezdje:97304b2e4c20015c0171cadf604804e68fafd4f9bc7fc9684a784bd9c3ce422a@ec2-18-215-111-67.compute-1.amazonaws.com:5432/d8phvec1vrp4cv

*postgres:// USERNAME : PASSWORD @ HOST : PORT : DATABASE_NAME*)
```

- `heroku config:set DATABASE_PORT=5432`

- `heroku config:set DATABASE_USERNAME=liaxabdytezdje`

- `heroku config:set DATABASE_PASSWORD=97304b2e4c20015c0171cadf604804e68fafd4f9bc7fc9684a784bd9c3ce422a`

- `heroku config:set DATABASE_HOST=ec2-18-215-111-67.compute-1.amazonaws.com`

- `heroku config:set DATABASE_NAME=d8phvec1vrp4c`

- `heroku config:set NODE_ENV=production`

- `heroku config:set MY_HEROKU_URL=$(heroku info -s | grep web_url | cut -d= -f2)`

- `heroku config:set CLOUDINARY_NAME=luisvalgoi`

- `heroku config:set CLOUDINARY_KEY=687372721644557`

- `heroku config:set CLOUDINARY_SECRET=BRKji3pGYTM3NOT_2ZZTnWm_3ZM`

https://strapi.io/documentation/developer-docs/latest/setup-deployment-guides/deployment/hosting-guides/heroku.html#heroku

## 👤 Users

- luisvalgoi@gmail.com | Initial1! | ADMIN

- bruna.ferri@outlook.com | Initial1! | EDITOR

## ℹ️  Notes

- It runs the `http://localhost:1337`

- It uses the `Cloudinary` as the image provider

- It uses `sqlite` for local database

- It uses `postgres` for production database

- `what is a User ?`: A person which access the app through the frontend.

- `what is a Admin ?`: A person which access the backend app of strapi. It has to access the admin portal / page.

## 🚀 Commands Line Interface

For more, access [this link here](https://strapi.io/documentation/developer-docs/latest/developer-resources/cli/CLI.html#command-line-interface-cli).

- `strapi start`: Start a Strapi application with autoReload disabled.

- `strapi develop`: Starts your application with the autoReload enabled.

- `strapi develop --watch-admin`: Starts your application with the autoReload enabled and the front-end development server. It allows you to customize the administration panel.

- `strapi build`: Builds the administration panel and minimizing the assets.

- `strapi build --clean`: Builds the administration panel and delete the previous build and .cache folders.
