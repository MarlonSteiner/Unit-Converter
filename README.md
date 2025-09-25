# 🔄 Ruby Unit Converter

A web-based unit conversion application built with Ruby 💎 and Sinatra, featuring a clean Bootstrap UI for converting between various units of measurement.

## ✨ Features

- **📏 Length Conversion**: Meters (m), kilometers (km), inches (in), feet (ft), yards (yd), miles (mi)
- **⚖️ Mass Conversion**: Grams (g), kilograms (kg), pounds (lb), ounces (oz), stones (st)
- **🧪 Volume Conversion**: Liters (L), milliliters (mL), gallons (gal), quarts (qt), pints (pt), cups (c)
- **📐 Area Conversion**: Square meters (m²), square kilometers (km²), square feet (ft²), acres (ac), hectares (ha)
- **🚀 Speed Conversion**: Meters per second (m/s), kilometers per hour (km/h), miles per hour (mph), knots (kn)
- **⏰ Time Conversion**: Seconds (s), minutes (min), hours (h), days (d), weeks (w), months (mo), years (y)
- **🌡️ Temperature Conversion**: Celsius (°C), Fahrenheit (°F), Kelvin (K)
- **📱 Responsive Design**: Mobile-friendly Bootstrap interface
- **⚡ Real-time Conversion**: Instant results as you type
- **✅ Input Validation**: Error handling for invalid inputs
- **🎨 Clean UI**: Modern, intuitive user interface

## 📋 Requirements

- Ruby 💎 2.7 or higher
- Bundler 📦 gem

## 🚀 Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/ruby-unit-converter.git
cd ruby-unit-converter

# Install dependencies
bundle install

# Start the application
ruby app.rb
```

Open your browser and navigate to `http://localhost:4567` 🌐 to use the application.

## 🧪 Running Tests

```bash
# Run the test suite
ruby test/test_converter.rb

# Or if using RSpec
bundle exec rspec
```

## 📁 Project Structure

```
ruby-unit-converter/
├── 📄 app.rb                 # Main Sinatra application
├── 📂 lib/
│   └── 🔧 converter.rb       # Unit conversion logic
├── 📂 views/
│   ├── 🎨 layout.erb         # Main layout template
│   ├── 🏠 index.erb          # Homepage with conversion form
│   └── 📊 result.erb         # Conversion results display
├── 📂 public/
│   ├── 📂 css/
│   │   └── 🎨 style.css      # Custom styles
│   ├── 📂 js/
│   │   └── ⚡ app.js         # Client-side JavaScript
│   └── 📂 images/
│       └── 🔖 favicon.ico    # Site favicon
├── 📂 test/
│   ├── 🧪 test_converter.rb  # Unit tests for conversion logic
│   └── 🧪 test_app.rb        # Integration tests for web app
├── 📦 Gemfile                # Ruby dependencies
├── 🔒 Gemfile.lock           # Locked dependency versions
└── 📖 README.md              # This file
```

## ⚙️ How It Works

The application follows a simple MVC pattern:

1. **🧠 Model (lib/converter.rb)**: Contains all unit conversion logic with precise conversion factors
2. **👁️ View (views/*.erb)**: ERB templates styled with Bootstrap for responsive design
3. **🎛️ Controller (app.rb)**: Sinatra routes handling HTTP requests and responses

The conversion engine uses a base unit system where each unit type has a reference unit (e.g., meters for length, grams for mass) and conversion factors are applied to convert between units accurately.

Key conversion examples:
- **📏 Length**: All conversions go through meters (m) as the base unit
- **🌡️ Temperature**: Handles the complex conversions between °C, °F, and K
- **🧪 Volume**: Supports both metric and imperial systems with precise conversions

## 📸 Screenshots

*Add screenshots of your application here showing:*
- 🖥️ Main conversion interface
- 📱 Different unit categories
- 📲 Mobile responsive design
- 📊 Conversion results display

## 🎬 Demo Video

*Link to a demo video showing the application in action*

## 📄 License

MIT License ⚖️

Copyright (c) 2025 [Your Name]

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

- Built with [Ruby 💎](https://www.ruby-lang.org/) and [Sinatra 🎤](http://sinatrarb.com/)
- UI styled with [Bootstrap 🅱️](https://getbootstrap.com/)
- Icon fonts from [Font Awesome 🎨](https://fontawesome.com/)
- Conversion factors verified against international standards 📏

---

**🤝 Contributing**: Feel free to submit issues and pull requests to improve this application.

**👨‍💻 Author**: Marlon Steiner
