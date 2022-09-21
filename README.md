# Blog app

> This blog App is used to create posts where users can like and comment. It uses ruby on rails and postgresql.

## Built With

- Ruby

## Getting Started

To use this application, you have to install ```Ruby```, then ```Ruby on rails``` clone this project using ```git clone https://github.com/JoffreyNK/blogs-app``` and install the depencancies using ```bundle install``` 
and the you will need postgresql database log in it and create `blogs` database manually
and after you need to create fields using the following commands

first run:  ```rails generate model user name:string photo:string bio:text post_counter:integer```

second: ```rails generate model post title:string text:text comments_counter:integer likes_counter:integer user:references```

third: ```rails generate model like post:references user:references```

fourth: ```rails generate model comment  text:text post:references user:references```

now run ```rails db:migrate```


## Authors

👤 **Joffrey**

- GitHub: [@joffreynk](https://github.com/joffreynk)
- Twitter: [@joffreynk](https://twitter.com/joffreynk)
- LinkedIn: [joffreynk](https://linkedin.com/in/joffreynk)


## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](../../issues/).

## Show your support

Give a ⭐️ if you like this project!

## Acknowledgments

- Hat tip to anyone whose code was used
- Inspiration
- etc

## 📝 License

This project is [MIT](./LICENSE) licensed.

_NOTE: we recommend using the [MIT license](https://choosealicense.com/licenses/mit/) - you can set it up quickly by [using templates available on GitHub](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository). You can also use [any other license](https://choosealicense.com/licenses/) if you wish._
