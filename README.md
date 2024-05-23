# Depot
Depot is an e-commerce application built with Ruby on Rails, following the guidelines and examples provided in the book *Agile Web Development with Rails 7* by Same Ruby with Dave Thomas.

## Prerequisites
- **Ruby**: 3.2.3
- **Rails**: 7.1.3.3
- **Database**: SQLite 3

## Getting Started
To get started with the Depot App, follow these steps:

1. **Clone the repository**

```sh
git clone https://github.com/Sp0k/depot_app.git depot
cd depot
```

2. **Install dependencies**

```sh
bundle install
```

3. **Build the project and start the server**

```sh
bin/dev
```

\* The project is set up to use the port 3001 on my machine, however you can fix that by changing 3001 to 3000 in the file *Procfile.dev* if you'd rather use the default port:

```dev
web: bin/rails server -p 3000
css: bin/rails tailwindcss:watch
```

4. **Visit the application in your browser**

Open your browser and navigate to `http://localhost:3001`. (or 3000 if you changed it)

## Development
### Running Tests
To run the test suite, execute:

```sh
bin/rails test
```

### Code Style
This project follows the Ruby style guide. To check the code style, run:

```sh
rubocop
```

## Deployment
To deploy the application, follow these steps:
1. **Set up the production database**

```sh
bin/rails db:setup RAILS_ENV=production
```

2. **Precompile assets**

```sh
bin/rails assets:precompile
```

3. **Start the server**

Ensure you have a web server like Puma, Unicorn, or Passenger set up for production.

## Contribution
Bug reports and pull requests are welcome on GitHub at https://github.com/Sp0k/depot_app.git. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](https://www.contributor-covenant.org/).

## License
The gem is available as open source under the terms of the [MIT License](LICENSE).