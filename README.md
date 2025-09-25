# 🔄 Ruby Unit Converter

A web-based unit conversion application built with Ruby on Rails, featuring a clean Bootstrap UI for converting between various units of measurement.

## ✨ Features

- **Length Conversion**: Meters (m), kilometers (km), inches (in), feet (ft), yards (yd), miles (mi)
- **Mass Conversion**: Grams (g), kilograms (kg), pounds (lb), ounces (oz), stones (st)
- **Volume Conversion**: Liters (L), milliliters (mL), gallons (gal), quarts (qt), pints (pt), cups (c)
- **Area Conversion**: Square meters (m²), square kilometers (km²), square feet (ft²), acres (ac), hectares (ha)
- **Speed Conversion**: Meters per second (m/s), kilometers per hour (km/h), miles per hour (mph), knots (kn)
- **Time Conversion**: Seconds (s), minutes (min), hours (h), days (d), weeks (w), months (mo), years (y)
- **Temperature Conversion**: Celsius (°C), Fahrenheit (°F), Kelvin (K)
- **Responsive Design**: Mobile-friendly Bootstrap interface
- **Real-time Conversion**: Instant results as you type
- **Input Validation**: Error handling for invalid inputs
- **Clean UI**: Modern, intuitive user interface

## 📋 Requirements

- Ruby 3.0 or higher
- Rails 7.0 or higher
- SQLite3 (default database)

## 🚀 Setup

```bash
# Clone the repository
git clone https://github.com/MarlonSteiner/Unit-Converter.git
cd Unit-Converter

# Install dependencies
bundle install

# Set up the database
rails db:create
rails db:migrate

# Start the application
rails server
```

Open your browser and navigate to `http://localhost:3000` to use the application.

## 🧪 Running Tests

```bash
# Run the test suite
rails test

# Or run specific tests
rails test test/controllers/conversions_controller_test.rb
rails test test/models/conversion_test.rb
```

## 📁 Project Structure

```
Unit-Converter/
├── app/
│   ├── controllers/
│   │   ├── application_controller.rb
│   │   └── conversions_controller.rb    # Main conversion logic
│   ├── models/
│   │   ├── application_record.rb
│   │   └── conversion.rb               # Conversion model & logic
│   ├── views/
│   │   ├── layouts/
│   │   │   └── application.html.erb   # Main layout template
│   │   └── conversions/
│   │       ├── index.html.erb         # Homepage with conversion form
│   │       └── convert.html.erb       # Conversion results display
│   └── assets/
│       ├── stylesheets/
│       │   └── application.scss       # Bootstrap + custom styles
│       └── javascripts/
│           └── application.js          # Rails + custom JS
├── config/
│   ├── routes.rb                      # URL routing
│   └── database.yml                   # Database configuration
├── db/
│   ├── schema.rb                      # Database schema
│   └── migrate/                       # Database migrations
├── test/
│   ├── controllers/
│   │   └── conversions_controller_test.rb
│   ├── models/
│   │   └── conversion_test.rb
│   └── fixtures/
│       └── conversions.yml
├── Gemfile                            # Ruby dependencies
├── Gemfile.lock                       # Locked dependency versions
└── README.md                          # This file
```

## ⚙️ How It Works

The application follows the Rails MVC pattern:

1. **Model (app/models/conversion.rb)**: Contains all unit conversion logic with precise conversion factors
2. **View (app/views/conversions/)**: ERB templates styled with Bootstrap for responsive design
3. **Controller (app/controllers/conversions_controller.rb)**: Rails controller handling HTTP requests and responses

The conversion engine uses a base unit system where each unit type has a reference unit (e.g., meters for length, grams for mass) and conversion factors are applied to convert between units accurately.

Key conversion examples:
- **Length**: All conversions go through meters (m) as the base unit
- **Temperature**: Handles the complex conversions between °C, °F, and K
- **Volume**: Supports both metric and imperial systems with precise conversions

## 📸 Screenshots

*Add screenshots of your application here showing:*
- Main conversion interface
- Different unit categories
- Mobile responsive design
- Conversion results display

## 🎬 Demo Video

*Link to a demo video showing the application in action*

## 📄 License

MIT License

Copyright (c) 2025 Marlon Steiner

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## 🙏 Credits

- Built with [Ruby](https://www.ruby-lang.org/) and [Rails](https://rubyonrails.org/)
- UI styled with [Bootstrap](https://getbootstrap.com/)
- Icon fonts from [Font Awesome](https://fontawesome.com/)
- Conversion factors verified against international standards

---

**Contributing**: Feel free to submit issues and pull requests to improve this application.

**Author**: Marlon Steiner ([marlon@example.com](mailto:marlon@example.com))
